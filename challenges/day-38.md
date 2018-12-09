## Problem

[https://www.hackerrank.com/challenges/text-wrap/problem](https://www.hackerrank.com/challenges/text-wrap/problem)

## Code

```py
def wrap(string, max_width):
    return '\n'.join([string[i:i+max_width] for i in range(0, len(string), max_width)])
```