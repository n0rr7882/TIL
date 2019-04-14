## Problem

[https://www.acmicpc.net/problem/2439](https://www.acmicpc.net/problem/2439)

## Source

```py
m = int(input())
for i in range(m):
    print(' ' * (m - i - 1), end='')
    print('*' * (i + 1))
```