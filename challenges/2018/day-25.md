## Problem

[https://www.hackerrank.com/challenges/swap-case/problem](https://www.hackerrank.com/challenges/swap-case/problem)

## Code

```py
def swap_case(s):
    return ''.join([i.lower() if i.isupper() else i.upper() for i in s])

if __name__ == '__main__':
    s = input()
    result = swap_case(s)
    print(result)
```