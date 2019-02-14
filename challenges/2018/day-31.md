## Problem

[https://www.hackerrank.com/challenges/30-2d-arrays/problem](https://www.hackerrank.com/challenges/30-2d-arrays/problem)

## Code

```py
#!/bin/python3

import math
import os
import random
import re
import sys



if __name__ == '__main__':
    arr = []

    for _ in range(6):
        arr.append(list(map(int, input().rstrip().split())))

    m = -99999999

    for i in range(4):
        for j in range(4):
            s = (
                arr[i][j]
                + arr[i][j + 1]
                + arr[i][j + 2]
                + arr[i + 1][j + 1]
                + arr[i + 2][j]
                + arr[i + 2][j + 1]
                + arr[i + 2][j + 2]
            )
            m = s if s > m else m
    
    print(m)
```