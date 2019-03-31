## Problem

[https://www.acmicpc.net/problem/2941](https://www.acmicpc.net/problem/2941)

## Source

```py
import re
r = re.compile(r'c=|c-|dz=|d-|lj|nj|s=|z=')
print(len(r.sub('*', input())))
```