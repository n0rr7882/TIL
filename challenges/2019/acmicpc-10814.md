## Problem

[https://www.acmicpc.net/problem/10814](https://www.acmicpc.net/problem/10814)

## Source

```py
users = []

for _ in range(int(input())):
    age, name = input().split()
    users.append({'age': int(age), 'name': name})

users = sorted(users, key=lambda x: x['age'])

for x in users:
    print('{} {}'.format(x['age'], x['name']))
```
