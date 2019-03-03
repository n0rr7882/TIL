## Problem

[https://www.acmicpc.net/problem/8958](https://www.acmicpc.net/problem/8958)

## Source

```py
for _ in range(int(input())):
    s_lst = input().split('X')
    score = 0
    for s in s_lst:
        for i in range(len(s)):
            score += (i + 1)
    print(score)
```