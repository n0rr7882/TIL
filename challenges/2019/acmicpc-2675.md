## Problem

[https://www.acmicpc.net/problem/2675](https://www.acmicpc.net/problem/2675)

## Source

```py
for _ in range(int(input())):
    n, s = input().split()
    for c in s:
        print(c * int(n), end='')
    print()
```