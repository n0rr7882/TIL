## Problem

[https://www.hackerrank.com/challenges/30-queues-stacks/problem](https://www.hackerrank.com/challenges/30-queues-stacks/problem)

## Code

```py
import sys

class Solution:
    _queue = []
    _stack = []

    def pushCharacter(self, item):
        self._stack.append(item)
    
    def popCharacter(self):
        return self._stack.pop()
    
    def enqueueCharacter(self, item):
        self._queue.insert(0, item)

    def dequeueCharacter(self):
        return self._queue.pop()

# read the string s
s=input()
#Create the Solution class object
obj=Solution()   

l=len(s)
# push/enqueue all the characters of string s to stack
for i in range(l):
    obj.pushCharacter(s[i])
    obj.enqueueCharacter(s[i])
    
isPalindrome=True
'''
pop the top character from stack
dequeue the first character from queue
compare both the characters
''' 
for i in range(l // 2):
    if obj.popCharacter()!=obj.dequeueCharacter():
        isPalindrome=False
        break
#finally print whether string s is palindrome or not.
if isPalindrome:
    print("The word, "+s+", is a palindrome.")
else:
    print("The word, "+s+", is not a palindrome.")    
```