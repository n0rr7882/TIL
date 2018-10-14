## Problem

* [https://www.hackerrank.com/challenges/30-conditional-statements/problem](https://www.hackerrank.com/challenges/30-conditional-statements/problem)

## Code

```py
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    N = int(input())

    if N % 2 != 0 or 6 <= N <= 20:
        print('Weird')
    else:
        print('Not Weird')
```
