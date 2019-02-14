## Problem
[https://www.hackerrank.com/challenges/30-exceptions-string-to-integer/problem](https://www.hackerrank.com/challenges/30-exceptions-string-to-integer/problem)

## Code

```py
#!/bin/python

import sys


S = raw_input().strip()

try:
    r = int(S)
    print(r)
except Exception:
    print('Bad String')
```