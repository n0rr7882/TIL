## Problem

[https://www.hackerrank.com/challenges/word-order/problem](https://www.hackerrank.com/challenges/word-order/problem)

## Code

```py
from collections import Counter, OrderedDict

class OrderedCounter(Counter, OrderedDict):
    pass

d = OrderedCounter(input() for _ in range(int(input())))
print(len(d))
print(*d.values())
```