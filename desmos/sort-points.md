# Sorting of Points

| | |
|--|--|
| | $$p = [(1,0),(3,1),(2,2)]$$ |
| | $$p_c = \text{sort}(p.x)$$ |
| | $$[(x,B(x)) \text{ for } x=p_c]$$ |
| | $$B(x) = \displaystyle\sum_{i=1}^n p[i].y \cdot k(p[i].x,x)$$ |
| | $$n = \text{length}(p)$$ |
| | $$k(i,j) = \\{ i=j: 1, 0 \\}$$ |
