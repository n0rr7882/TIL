## Problem

* [https://www.hackerrank.com/challenges/30-class-vs-instance/problem](https://www.hackerrank.com/challenges/30-class-vs-instance/problem)

## Code

```py
class Person:
    def __init__(self,initialAge):
        # Add some more code to run some checks on initialAge
        if initialAge < 0:
            print('Age is not valid, setting age to 0.')
            initialAge = 0
        self.age = initialAge

    def amIOld(self):
        # Do some computations in here and print out the correct statement to the console
        if self.age < 13:
            print('You are young.')
        elif self.age < 18:
            print('You are a teenager.')
        else:
            print('You are old.')

    def yearPasses(self):
        # Increment the age of the person in here
        self.age += 1
```
