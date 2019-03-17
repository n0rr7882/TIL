## Problem

[https://www.acmicpc.net/problem/5622](https://www.acmicpc.net/problem/5622)

## Source

```py
dial = ['ABC', 'DEF', 'GHI', 'JKL', 'MNO', 'PQRS', 'TUV', 'WXYZ']
offset = 3

result = 0
for c in input():
    for i in range(len(dial)):
        if c in dial[i]:
            result += (i + offset)
            continue
print(result)
```