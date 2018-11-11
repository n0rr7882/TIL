## Problem

[https://www.hackerrank.com/challenges/weather-observation-station-5/problem](https://www.hackerrank.com/challenges/weather-observation-station-5/problem)

## Code

```sql
SELECT CITY,LENGTH(CITY) FROM STATION WHERE LENGTH(CITY) = (
    SELECT MIN(LENGTH(CITY)) FROM STATION
) ORDER BY CITY LIMIT 1;
SELECT CITY,LENGTH(CITY) FROM STATION WHERE LENGTH(CITY) = (
    SELECT MAX(LENGTH(CITY)) FROM STATION
) ORDER BY CITY LIMIT 1;
```