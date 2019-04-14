## Problem

[https://www.acmicpc.net/problem/15552](https://www.acmicpc.net/problem/15552)

## Source

```py
import sys
for _ in range(int(input())):
    A, B = sys.stdin.readline().rstrip().split()
    print(int(A) + int(B))
```