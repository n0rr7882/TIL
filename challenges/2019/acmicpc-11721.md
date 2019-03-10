## Problem

[https://www.acmicpc.net/problem/11721](https://www.acmicpc.net/problem/11721)

## Source

```py
i = 1
for c in input():
    print(c, end='')
    if i % 10 == 0:
        print()
    i += 1
```