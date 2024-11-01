# Distance Between 2 Points on Earth

* [Haversine Formula](https://en.wikipedia.org/wiki/Haversine_formula)
* [UTM Coordinate System](https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system)

---
$$
D(A,B) = 6371c
$$

where:

$$
\begin{array}{l}
c = 2\arctan_2(\sqrt{a},\sqrt{1-a})
\\
a = \sin^2\left(
 \frac{\varphi_{\Delta}}{2}
\right) + n \sin^2\left(
 \frac{\lambda_{\Delta}}{2}
\right)
\\
n = \cos(A_{\text{lat}}) \cos(B_{\text{lat}})
\\
\varphi_{\Delta} = B_{\text{lat}}-A_{\text{lat}}
\\
\lambda_{\Delta} = B_{\text{lon}}-A_{\text{lon}}
\end{array}
$$

## JavaScript Implementation

```
function getDistance(A, B) {
  const rad = n => n * Math.PI / 180;
  const [lat1,lon1] = A.map(rad);
  const [lat2,lon2] = B.map(rad);
  
  const sin2 = x => Math.sin(x)**2;
  const R = 6371; // radius of Earth (KM)

  const latDelta = lat2 - lat1;
  const lonDelta = lon2 - lon1;

  const n = Math.cos(lat1) * Math.cos(lat2);
  const a =
    sin2(latDelta / 2) +
    sin2(lonDelta / 2) * n;

  const c = 2 * Math.atan2(
    Math.sqrt(a),
    Math.sqrt(1 - a)
  );
  const d = R * c;

  return +d.toFixed(2); // KM
}
```

```
const tokyo = [35.6895, 139.69171];
const sydney = [-33.86785, 151.20732];

console.log(
  getDistance(tokyo, sydney)
);
// 7826.48
// (7821 KM by Google)


const warsaw = [52.22977, 21.01178];
const poznan = [52.40692, 16.92993];

console.log(
  getDistance(warsaw, poznan)
);
// 278.11
// (278.34 KM by Google Maps)
```

> Coordinates from:
> [https://public.opendatasoft.com/explore/dataset/geonames-all-cities-with-a-population-1000/table](https://public.opendatasoft.com/explore/dataset/geonames-all-cities-with-a-population-1000/table/?disjunctive.cou_name_en&sort=name)


