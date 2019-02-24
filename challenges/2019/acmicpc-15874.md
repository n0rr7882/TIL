## Problem

[https://www.acmicpc.net/problem/15874](https://www.acmicpc.net/problem/15874)

## Source

```py
L2I = dict(zip("abcdefghijklmnopqrstuvwxyz",range(26)))
I2L = dict(zip(range(26),"abcdefghijklmnopqrstuvwxyz"))

key, _ = map(int, input().split())

plaintext = input()

encrypted = ""
for c in plaintext:
    if c.isalpha():
        isupper = c.isupper()
        if isupper: c = c.lower()
        c = I2L[(L2I[c] + key) % 26]
        if isupper: c = c.upper()
    encrypted += c
    
print(encrypted)
```
