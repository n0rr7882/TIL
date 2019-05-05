## Problem

[https://www.acmicpc.net/problem/2839](https://www.acmicpc.net/problem/2839)

## Source

```py
n = int(input())
F = int(n / 5)
n %= 5
T = 0
while F >= 0:
    if n % 3 == 0:
        T = int(n / 3)
        n = int(n % 3)
        break
    F -= 1
    n += 5
print((n == 0) and (F + T) or -1)
```