## Problem

[https://www.acmicpc.net/problem/2857](https://www.acmicpc.net/problem/2857)

## Source

```py
exists = False
for i in range(5):
    if 'FBI' in input():
        print(i + 1, end=' ')
        exists = True
if not exists: print('HE GOT AWAY!')
```