## Problem

[https://www.hackerrank.com/challenges/30-review-loop/problem](https://www.hackerrank.com/challenges/30-review-loop/problem)

## Code

```py
r = int(input())

for _ in range(r):
    s = input()
    r1 = ''
    r2 = ''
    for i in range(len(s)):
        if i % 2 == 0:
            r1 += s[i]
        else:
            r2 += s[i]
    print('{} {}'.format(r1, r2))
```