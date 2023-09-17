# Day #08 - Weather Observation Station 2
## Problem

Query the following two values from the **STATION** table:

1. The sum of all values in LAT_N rounded to a scale of **2** decimal places.
2. The sum of all values in LONG_W rounded to a scale of **2** decimal places.

***Input Format***

The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/92add95f-9d84-4083-8e53-50d97ad1190d)


where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

***Output Format***

Your results must be in the form:
```

lat lon

```
where **lat** is the sum of all values in LAT_N and **lon** is the sum of all values in LONG_W. Both results must be rounded to a scale of  decimal places.

## Solution
```sql
SELECT
    ROUND(SUM(lat_n), 2), 
    ROUND(SUM(long_w), 2)
FROM station
```
