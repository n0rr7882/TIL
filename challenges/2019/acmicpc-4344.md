## Problem

[https://www.acmicpc.net/problem/4344](https://www.acmicpc.net/problem/4344)

## Source

```py
for _ in range(int(input())):
    score_list = list(map(int, input().split()))[1:]
    score_len = len(score_list)
    score_sum = sum(score_list)
    score_avg = score_sum / float(score_len)
    pass_list = list(filter(lambda x: x > score_avg, score_list))
    pass_len = len(pass_list)
    print('%.3f' % ((pass_len / float(score_len)) * 100) + '%')
```