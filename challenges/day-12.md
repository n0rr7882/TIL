## Problem

[https://www.hackerrank.com/challenges/detect-html-tags-attributes-and-attribute-values/problem](https://www.hackerrank.com/challenges/detect-html-tags-attributes-and-attribute-values/problem)

## Code

```py
from html.parser import HTMLParser

class MyHTMLParser(HTMLParser):
    def handle_starttag(self, tag, attrs):
        print(tag)
        for attr in attrs:
            print('-> ' + attr[0] + ' > ' + attr[1])
            
html = '\n'.join([input() for _ in range(int(input()))])
MyHTMLParser().feed(html)
```