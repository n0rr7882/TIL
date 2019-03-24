## Problem

[https://www.acmicpc.net/problem/2441](https://www.acmicpc.net/problem/2441)

## Source

```py
c = int(input())
for i in range(c):
    print(' ' * i, end='')
    print('*' * (c - i))
```