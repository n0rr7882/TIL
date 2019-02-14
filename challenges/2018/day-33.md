## Problem

[https://www.hackerrank.com/challenges/30-inheritance/problem](https://www.hackerrank.com/challenges/30-inheritance/problem)

## Code

```py
class MyBook(Book):
    def __init__(self, title, author, price):
        Book.__init__(self, title, author)
        self.price = price

    def display(self):
        print("Title: {}".format(self.title))
        print("Author: {}".format(self.author))
        print("Price: {}".format(self.price))
```