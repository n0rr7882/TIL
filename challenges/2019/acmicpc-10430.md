## Problem

[https://www.acmicpc.net/problem/10430](https://www.acmicpc.net/problem/10430)

## Source

```py
A, B, C = map(int, input().split())
print((A+B)%C)
print((A%C + B%C)%C)
print((A*B)%C)
print((A%C * B%C)%C)
```