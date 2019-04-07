## Problem

[https://www.acmicpc.net/problem/10871](https://www.acmicpc.net/problem/10871)

## Source

```py
_, X = map(int, input().split())
print(' '.join(map(str, filter(lambda x: x < X, map(int, input().split())))))
```