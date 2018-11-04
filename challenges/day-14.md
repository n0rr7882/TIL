## Problem

[https://www.hackerrank.com/challenges/30-sorting/problem](https://www.hackerrank.com/challenges/30-sorting/problem)

## Code

```py
#!/bin/python3

import sys

n = int(input().strip())
a = list(map(int, input().strip().split(' ')))
# Write Your Code Here
c = 0

length = len(a)-1
for i in range(length):
    for j in range(length-i):
        if a[j] > a[j+1]:
            c += 1
            a[j], a[j+1] = a[j+1], a[j]
            
print('Array is sorted in {} swaps.'.format(c))
print('First Element: {}'.format(a[0]))
print('Last Element: {}'.format(a[n - 1]))
```
