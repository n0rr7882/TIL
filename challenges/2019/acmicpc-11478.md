## Problem

[https://www.acmicpc.net/problem/11478](https://www.acmicpc.net/problem/11478)

## Source

```py
S = input()
L = []
for i in range(len(S)):
    for j in range(i, len(S)):
        L.append(S[i:j+1])
print(len(set(L)))
```