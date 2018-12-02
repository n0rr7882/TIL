## Problem

[https://www.hackerrank.com/challenges/30-binary-numbers/problem](https://www.hackerrank.com/challenges/30-binary-numbers/problem)

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
    b = bin(n)[2:]

    print(len(max(b.split('0'), key=len)))
    
```