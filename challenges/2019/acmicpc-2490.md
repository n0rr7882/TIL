## Problem

[https://www.acmicpc.net/problem/2490](https://www.acmicpc.net/problem/2490)

## Source

```py
Y = ['D', 'C', 'B', 'A', 'E']
for _ in range(3):
    S = sum(map(int, input().split()))
    print(Y[S])
```