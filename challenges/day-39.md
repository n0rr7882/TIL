## Problem

[https://www.hackerrank.com/challenges/python-time-delta/problem](https://www.hackerrank.com/challenges/python-time-delta/problem)

## Code

```py
from datetime import datetime as dt

def time_delta(t1, t2):
    fmt = '%a %d %b %Y %H:%M:%S %z'
    return '{}'.format(int(abs((dt.strptime(t1, fmt) - 
                                dt.strptime(t2, fmt)).total_seconds())))
```