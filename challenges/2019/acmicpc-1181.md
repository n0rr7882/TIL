## Problem

[https://www.acmicpc.net/problem/1181](https://www.acmicpc.net/problem/1181)

## Source

```py
l = []
for _ in range(int(input())):
    l.append(input())

l = list(set(l))
l.sort()
l.sort(key=len)

for s in l:
    print(s)
```