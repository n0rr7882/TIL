## Problem

[https://www.hackerrank.com/challenges/30-interfaces/problem](https://www.hackerrank.com/challenges/30-interfaces/problem)

## Code

```py
class AdvancedArithmetic(object):
    def divisorSum(n):
        raise NotImplementedError

class Calculator(AdvancedArithmetic):
    def divisorSum(self, n):
        t = 0
        for i in range(n):
            if n % (i + 1) == 0:
                t += (i + 1)
        return t


n = int(input())
my_calculator = Calculator()
s = my_calculator.divisorSum(n)
print("I implemented: " + type(my_calculator).__bases__[0].__name__)
print(s)
```