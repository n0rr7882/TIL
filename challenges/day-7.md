## Problem

[https://www.hackerrank.com/challenges/30-arrays/problem](https://www.hackerrank.com/challenges/30-arrays/problem)

## Code

```py
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    n = int(input())

    arr = list(map(str, input().rstrip().split()))
    arr.reverse()
    print(' '.join(arr))
```