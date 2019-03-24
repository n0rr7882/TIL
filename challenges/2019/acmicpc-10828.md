## Problem

[https://www.acmicpc.net/problem/10828](https://www.acmicpc.net/problem/10828)

## Source

```py
class Stack:
    s = []
    def push(self, v): self.s.append(v)
    def pop(self): print(self.s.pop())
    def size(self): print(len(self.s))
    def empty(self): print(0 if len(self.s) > 0 else 1)
    def top(self): print(self.s[-1] if len(self.s) > 0 else -1)
    def do(self, i):
        t = i[0]
        if t == 'push': self.push(int(i[1]))
        elif t == 'pop': self.pop()        
        elif t == 'size': self.size()
        elif t == 'empty': self.empty()
        elif t == 'top': self.top()
s = Stack()
for _ in range(int(input())):
    s.do(input().split())
```