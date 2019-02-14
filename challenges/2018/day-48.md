## Problem

[https://www.hackerrank.com/challenges/py-set-intersection-operation/problem](https://www.hackerrank.com/challenges/py-set-intersection-operation/problem)

## Code

```py
input()
s1 = set(map(int, input().split()))
input()
s2 = set(map(int, input().split()))

print(len(s1.intersection(s2)))
```