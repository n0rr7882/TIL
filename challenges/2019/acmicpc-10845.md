## Problem

[https://www.acmicpc.net/problem/10845](https://www.acmicpc.net/problem/10845)

## Source

```py
class Q:
    q = []
    def push(self, v): self.q.append(v)
    def pop(self):
        if len(self.q) > 0:
            v = self.q[0]
            self.q = self.q[1:]
        else:
            v = -1
        print(v)
    def size(self): print(len(self.q))
    def empty(self): print(0 if len(self.q) > 0 else 1)
    def front(self): print(self.q[0] if len(self.q) > 0 else -1)
    def back(self): print(self.q[-1] if len(self.q) > 0 else -1)
    def do(self, i):
        t = i[0]
        if t == 'push': self.push(int(i[1]))
        elif t == 'pop': self.pop()        
        elif t == 'size': self.size()
        elif t == 'empty': self.empty()
        elif t == 'front': self.front()
        elif t == 'back': self.back()
q = Q()
for _ in range(int(input())):
    q.do(input().split())
```