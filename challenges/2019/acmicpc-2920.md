## Problem

[https://www.acmicpc.net/problem/2920](https://www.acmicpc.net/problem/2920)

## Source

```py
S = input().replace(' ', '')
if S == '12345678':
    print('ascending')
elif S == '87654321':
    print('descending')
else:
    print('mixed')
```