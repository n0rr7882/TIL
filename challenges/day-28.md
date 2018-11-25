## Problem

[https://www.hackerrank.com/challenges/validating-credit-card-number/problem](https://www.hackerrank.com/challenges/validating-credit-card-number/problem)

## Code

```py
import re

for _ in range(int(input())):
    u = str(input())
    try:
        assert re.search(r'^[456]\d{3}(-?\d{4}){3}$', u)
        assert re.search(r'^((\d)-?(?!(-?\2){3})){16}$', u)
    except:
        print('Invalid')
    else:
        print('Valid')
```