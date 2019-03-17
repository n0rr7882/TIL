## Problem

[https://www.acmicpc.net/problem/2577](https://www.acmicpc.net/problem/2577)

## Source

```py
result = 1

for _ in range(3):
    result *= int(input())
    
result_list = list(str(result))

for i in range(10):
    print(result_list.count(str(i)))
```
