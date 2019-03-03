## Problem

[https://www.acmicpc.net/problem/12756](https://www.acmicpc.net/problem/12756)

## Source

```py
import math

att_a, def_a = tuple(map(int, input().split()))
att_b, def_b = tuple(map(int, input().split()))

a = math.ceil(def_a / att_b)
b = math.ceil(def_b / att_a)

if a > b:
    print('PLAYER A')
elif a < b:
    print('PLAYER B')
else:
    print('DRAW')
```