## Problem

[https://www.acmicpc.net/problem/1157](https://www.acmicpc.net/problem/1157)

## Source

```py
d = [0 for _ in range(26)]
m = 0
for c in input():
    o = (ord(c) - 65) % 32
    d[o] += 1
    if d[m] < d[o]: m = o
for i in range(len(d)):
    if i != m and d[i] == d[m]:
        print('?')
        break
if i == 25:
    print(chr(m + 65))
```