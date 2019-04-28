## Problem

[https://www.acmicpc.net/problem/2455](https://www.acmicpc.net/problem/2455)

## Source

```py
M, N = 0, 0
for _ in range(4):
    o, i = map(int, input().split())
    N = N + i - o
    if M < N: M = N
print(M)
```