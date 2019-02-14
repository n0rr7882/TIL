## Problem

[https://www.hackerrank.com/challenges/re-sub-regex-substitution/problem](https://www.hackerrank.com/challenges/re-sub-regex-substitution/problem)

## Code

```py
import re

for _ in range(int(input())):
    print(re.sub(r'(?<= )(&&|\|\|)(?= )',
          lambda x: 'and' if x.group() == '&&' else 'or',
          input()))
```