## Problem

[https://www.hackerrank.com/challenges/more-than-75-marks/problem](https://www.hackerrank.com/challenges/more-than-75-marks/problem)

## Code

```sql
SELECT name FROM STUDENTS WHERE marks > 75 ORDER BY SUBSTR(name, LENGTH(name) - 2, LENGTH(name)), id;
```