## Problem

[https://www.acmicpc.net/problem/2747](https://www.acmicpc.net/problem/2747)

## Source

```py
n = int(input())
a, b = 1, 0
for i in range(n):
    a, b = b, a + b
print(b)
```