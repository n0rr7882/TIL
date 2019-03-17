## Problem

[https://www.acmicpc.net/problem/2908](https://www.acmicpc.net/problem/2908)

## Source

```py
x, y = input().split()

x_rev = int(x[::-1])
y_rev = int(y[::-1])

if x_rev > y_rev:
    print(x_rev)
else:
    print(y_rev)
```