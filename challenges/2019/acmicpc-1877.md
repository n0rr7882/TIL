## Problem

[https://www.acmicpc.net/problem/1977](https://www.acmicpc.net/problem/1977)

## Source

```py
def get_PJ(N, M):
    r = []
    for i in range(101):
        pj = i * i
        if N <= pj <= M:
            r.append(pj)
    return r

N = int(input())
M = int(input())
r = get_PJ(N, M)
if r:
    print(sum(r))
    print(min(r))
else:
    print(-1)
```