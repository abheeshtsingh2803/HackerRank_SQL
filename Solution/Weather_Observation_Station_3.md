# Day #09 - Weather Observation Station 3
## Problem

Query a list of **CITY** names from **STATION** for cities that have an even **ID** number. Print the results in any order, but exclude duplicates from the answer.
The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/d2343831-c33a-46f6-b3e7-fc8ed9ea260c)


where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

## Solution
```sql
SELECT DISTINCT CITY FROM STATION
WHERE MOD(ID, 2) = 0;
```
