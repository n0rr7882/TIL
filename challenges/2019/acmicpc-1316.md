## Problem

[https://www.acmicpc.net/problem/1316](https://www.acmicpc.net/problem/1316)

## Source

```py
count = 0
for _ in range(int(input())):
    q = False
    s = ".%s." % input()
    for c in "abcdefghijklmnopqrstuvwxyz":
        if len(list(filter(lambda x: len(x) > 0, s.split(c)))) > 2:
            q = True
    if not q:
        count += 1
print(count)
```