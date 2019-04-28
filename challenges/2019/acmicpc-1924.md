## Problem

[https://www.acmicpc.net/problem/1924](https://www.acmicpc.net/problem/1924)

## Source

```py
S = [0, 31, 59, 90, 120, 151, 181, 212, 243, 273, 304, 334]
D = ['SUN', 'MON', 'TUE', 'WED', 'THU', 'FRI', 'SAT']
m, d = map(int, input().split())
s_m = S[m-1]
t = s_m + d
print(D[t % 7])
```