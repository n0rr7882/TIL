## Problem

[https://www.hackerrank.com/challenges/30-scope/problem](https://www.hackerrank.com/challenges/30-scope/problem)

## Code

```py
class Difference:
    def __init__(self, a):
        self.__elements = a

	# Add your code here
    def computeDifference(self):
        maximum = max(self.__elements)
        minimum = min(self.__elements)
        print(maximum - minimum)
```