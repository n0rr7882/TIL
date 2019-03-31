## Problem

[https://www.acmicpc.net/problem/10866](https://www.acmicpc.net/problem/10866)

## Source

```py
class D:
    d = []
    def push_front(self, v):
        self.d = [v] + self.d
    def push_back(self, v):
        self.d = self.d + [v]
    def pop_front(self):
        if len(self.d) > 0:
            v = self.d[0]
            self.d = self.d[1:]
        else:
            v = -1
        print(v)
    def pop_back(self):
        if len(self.d) > 0:
            v = self.d[-1]
            self.d = self.d[:-1]
        else:
            v = -1
        print(v)
    def size(self): print(len(self.d))
    def empty(self): print(0 if len(self.d) > 0 else 1)
    def front(self): print(self.d[0] if len(self.d) > 0 else -1)
    def back(self): print(self.d[-1] if len(self.d) > 0 else -1)
    def do(self, i):
        t = i[0]
        if t == 'push_front': self.push_front(int(i[1]))
        elif t == 'push_back': self.push_back(int(i[1]))
        elif t == 'pop_front': self.pop_front()
        elif t == 'pop_back': self.pop_back()
        elif t == 'size': self.size()
        elif t == 'empty': self.empty()
        elif t == 'front': self.front()
        elif t == 'back': self.back()
d = D()
for _ in range(int(input())):
    d.do(input().split())
```