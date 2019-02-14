## Problem

[https://www.hackerrank.com/challenges/30-loops/problem](https://www.hackerrank.com/challenges/30-loops/problem)

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
    
    for i in range(10):
        print('{} x {} = {}'.format(n, i + 1, n * (i + 1)))
```