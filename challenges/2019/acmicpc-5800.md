## Problem

[https://www.acmicpc.net/problem/5800](https://www.acmicpc.net/problem/5800)

## Source

```py
for i in range(int(input())):
    scores = sorted(list(map(int, input().split()))[1:])
    maximum = max(scores)
    minimum = min(scores)
    max_gap = 0
    for j in range(len(scores) - 1):
        current_gap = scores[j + 1] - scores[j]
        if current_gap > max_gap:
            max_gap = current_gap
    print('Class {}'.format(i + 1))
    print('Max {}, Min {}, Largest gap {}'.format(maximum, minimum, max_gap))
```
