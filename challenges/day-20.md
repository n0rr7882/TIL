## Problem

[https://www.hackerrank.com/challenges/weather-observation-station-10/problem](https://www.hackerrank.com/challenges/weather-observation-station-10/problem)

## Code

```sql
SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP ".*[^aeiou]$";
```