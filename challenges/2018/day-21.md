## Problem

[https://www.hackerrank.com/challenges/weather-observation-station-11/problem](https://www.hackerrank.com/challenges/weather-observation-station-11/problem)

## Code

```sql
SELECT DISTINCT CITY FROM STATION WHERE CITY REGEXP "(.*[^aeiou]$)|(^[^aeiou].*)";
```