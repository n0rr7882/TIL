## Problem

[https://www.acmicpc.net/problem/10039](https://www.acmicpc.net/problem/10039)

## Source

```py
t = 0
for _ in range(5):
    i = int(input())
    t += i if i > 40 else 40
print(t // 5)
```