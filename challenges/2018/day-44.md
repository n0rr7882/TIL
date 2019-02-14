## Problem

[https://www.hackerrank.com/challenges/finding-the-percentage/problem](https://www.hackerrank.com/challenges/finding-the-percentage/problem)

## Code

```py
if __name__ == '__main__':
    n = int(input())
    student_marks = {}
    for _ in range(n):
        name, *line = input().split()
        scores = list(map(float, line))
        student_marks[name] = scores
    query_name = input()
    total = sum(student_marks[query_name])
    avg = total / len(student_marks[query_name])
    print('%.2f' % avg)
```