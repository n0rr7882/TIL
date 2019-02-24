## Problem

[https://www.acmicpc.net/problem/1158](https://www.acmicpc.net/problem/1158)

## Source

```py
r, m = map(int, input().split())
q = list(range(1, r + 1))

c = 0
result = []
while len(q) > 0:
    c = (c + m - 1) % len(q)
    result.append(str(q.pop(c)))
    
print('<{}>'.format(', '.join(result)))
```