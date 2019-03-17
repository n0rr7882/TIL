## Problem

[https://www.acmicpc.net/problem/1110](https://www.acmicpc.net/problem/1110)

## Source

```py
original_value_str = input()

if len(original_value_str) == 1:
    original_value_str = '0' + original_value_str

current_value_str = original_value_str

count = 0

while True:
    
    count += 1
    
    cv_first = int(current_value_str[0])
    cv_last = int(current_value_str[1])
    
    new_cv_first = str(cv_last)
    new_cv_last = str(cv_first + cv_last)[-1]
    
    current_value_str = new_cv_first + new_cv_last
    
    if current_value_str == original_value_str:
        break
        
print(count)
```