## Problem

[https://www.hackerrank.com/challenges/py-introduction-to-sets/problem](https://www.hackerrank.com/challenges/py-introduction-to-sets/problem)

## Code

```py
def average(array):
    cleaned = list(set(array))
    return '%.3f' % (sum(cleaned) / len(cleaned))

if __name__ == '__main__':
    n = int(input())
    arr = list(map(int, input().split()))
    result = average(arr)
    print(result)
```