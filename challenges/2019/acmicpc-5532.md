## Problem

[https://www.acmicpc.net/problem/5532](https://www.acmicpc.net/problem/5532)

## Source

```py
L = int(input())
A = int(input())
B = int(input())
C = int(input())
D = int(input())

print(int(L - max((A / C, B / D))))
```