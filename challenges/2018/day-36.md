## Problem

[https://www.hackerrank.com/challenges/python-mutations/problem](https://www.hackerrank.com/challenges/python-mutations/problem)

## Code

```py
def mutate_string(string, position, character):
    return string[:position] + character + string[position+1:]
```