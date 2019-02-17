# Problem

[https://www.acmicpc.net/problem/1543](https://www.acmicpc.net/problem/1543)

# Source

```py
s = input()
k = input()
kl = len(k)
c = 0

while True:
    p = s.find(k)
    if p == -1:
        break
    c += 1
    s = s[:p] + ('*' * kl) + s[p + kl:]

print(c)
```