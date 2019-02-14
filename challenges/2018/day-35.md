## Problem

[https://www.hackerrank.com/challenges/capitalize/problem](https://www.hackerrank.com/challenges/capitalize/problem)

## Code

```py
def solve(s):
    sen = ' ' + s
    for i in range(len(sen)):
        if sen[i - 1] == ' ':
            sen = sen[:i] + sen[i].upper() + sen[i+1:]
    
    return sen[1:]
```