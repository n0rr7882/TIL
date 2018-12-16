## Problem

[https://www.hackerrank.com/challenges/30-scope/problem](https://www.hackerrank.com/challenges/30-scope/problem)

## Code

```py
class Difference:
    def __init__(self, a):
        self.__elements = a
    
    def computeDifference(self):
        self.maximumDifference = 0

        while len(self.__elements) > 0:
            t = self.__elements.pop()

            for e in self.__elements:
                r = (t - e) if (t - e) > 0 else (e - t)

                if self.maximumDifference < r:
                    self.maximumDifference = r

_ = input()
a = [int(e) for e in input().split(' ')]

d = Difference(a)
d.computeDifference()

print(d.maximumDifference)
```