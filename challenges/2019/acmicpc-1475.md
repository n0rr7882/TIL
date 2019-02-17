# Problem

[https://www.acmicpc.net/problem/1475](https://www.acmicpc.net/problem/1475)

# Source

```py
import math

s = input()
h = {}
for i in range(9):
    if i == 9 or i == 6:
        h['6'] = s.count('9') + s.count('6')
    else:
        h[str(i)] = s.count(str(i))
    
h['6'] = math.ceil(h['6'] / 2)

print(max(h.values()))
```