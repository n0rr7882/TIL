## Problem

[https://www.acmicpc.net/problem/1546](https://www.acmicpc.net/problem/1546)

## Source

```py
input()
S = list(map(int, input().split()))
M = max(S)
N = list(map(lambda x: x/M*100, S))
print(sum(N)/len(N))
```