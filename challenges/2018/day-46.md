## Problem

[https://www.hackerrank.com/challenges/maximum-element/problem](https://www.hackerrank.com/challenges/maximum-element/problem)

## Code

```py
class Stack:
    _stack = []

    def _push(self, item):
        self._stack.append(item)

    def _pop(self):
        return self._stack.pop()

    def _get_max(self):
        m = -9999999999999999999
        for i in self._stack:
            if m < i:
                m = i
        return m

    def do(self, op, operand):
        if op == 1:
            self._push(operand)
        elif op == 2:
            self._pop()
        elif op == 3:
            print(self._get_max())

if __name__ == '__main__':
    s = Stack()
    for _ in range(int(input())):
        r = str(input()).split()
        s.do(int(r[0]), int(r[1]) if len(r) > 1 else None)
```