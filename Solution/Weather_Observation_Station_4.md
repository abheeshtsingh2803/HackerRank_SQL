# Day #07 - Weather Observation Station 4
## Problem

Find the difference between the total number of **CITY** entries in the table and the number of distinct **CITY** entries in the table.
The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/92c15abd-722e-438e-b3e6-bad19cfe0c9f)


where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

## Solution
```sql
SELECT (COUNT(CITY) - COUNT(DISTINCT CITY)) FROM STATION;
```
