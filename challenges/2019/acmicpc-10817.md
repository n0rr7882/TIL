## Problem

[https://www.acmicpc.net/problem/10817](https://www.acmicpc.net/problem/10817)

## Source

```py
f, s ,t = map(int, input().split())
print(f if (s <= f <= t) or (t <= f <= s) else
      s if (f <= s <= t) or (t <= s <= f) else
      t)
```