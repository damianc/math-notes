# Distance Between 2 Points on Earth

* [Haversine Formula](https://en.wikipedia.org/wiki/Haversine_formula)
* [UTM Coordinate System](https://en.wikipedia.org/wiki/Universal_Transverse_Mercator_coordinate_system)

## Formula

$$
D(A,B) = 6371c
$$

where:

$$
\begin{array}{l}
c = 2\arctan_2(\sqrt{a},\sqrt{1-a})
\\
a = {\text{hav}}(\varphi_{\Delta}) + n \cdot {\text{hav}}(\lambda_{\Delta})
\\
n = \cos(A_{\text{lat}}) \cos(B_{\text{lat}})
\\
{\text{hav}}(x) = \sin^2\left(
 \frac{x}{2}
\right)
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
  const hav = x => Math.sin(x/2)**2;

  const [lat1,lon1] = A.map(rad);
  const [lat2,lon2] = B.map(rad);

  // radius of Earth (KM)
  const R = 6371;

  const latDelta = lat2 - lat1;
  const lonDelta = lon2 - lon1;

  const n = Math.cos(lat1) * Math.cos(lat2);
  const a = hav(latDelta) + n * hav(lonDelta);

  const c = 2 * Math.atan2(
    Math.sqrt(a),
    Math.sqrt(1 - a)
  );
  const d = R * c;

  // distance in KM
  return +d.toFixed(2);
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


