## Problem

[https://www.acmicpc.net/problem/9012](https://www.acmicpc.net/problem/9012)

## Source

```py
for _ in range(int(input())):
    c = 0
    S = input()
    for C in S:
        if C == '(':
            c += 1
        elif C == ')':
            c -= 1

        if c < 0:
            c = 9999999
    
    if c == 0:
        print('YES')
    else:
        print('NO')
```