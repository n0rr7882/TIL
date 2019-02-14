## Problem

[https://www.hackerrank.com/challenges/html-parser-part-1/problem](https://www.hackerrank.com/challenges/html-parser-part-1/problem)

## Code

```py
from html.parser import HTMLParser

class MyHTMLParser(HTMLParser):
    def handle_starttag(self, tag, attrs):
        print('Start : ' + tag)
        for attr in attrs:
            print('-> ' + str(attr[0]) + ' > ' + str(attr[1]))
    def handle_endtag(self, tag):
        print('End   : ' + tag)
    def handle_startendtag(self, tag, attrs):
        print('Empty : ' + tag)
        for attr in attrs:
            print('-> ' + str(attr[0]) + ' > ' + str(attr[1]))
            
parser = MyHTMLParser()

line = int(input())

for i in range(0, line):
    parser.feed(str(input()))
```