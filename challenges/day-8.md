## Problem

[https://www.hackerrank.com/challenges/30-dictionaries-and-maps/problem](https://www.hackerrank.com/challenges/30-dictionaries-and-maps/problem)

## Code

```py
r = int(input())

phone_book = {}

for _ in range(r):
    name, phone = input().split()
    phone_book[name] = phone

for _ in range(r):
    name = input()
    if name in phone_book:
        print('{}={}'.format(name, phone_book[name]))
    else:
        print('Not found')
```