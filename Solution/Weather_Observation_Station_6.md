# Day #12 - Weather Observation Station 6
## Problem

Query the list of **CITY** names starting with vowels (i.e., a, e, i, o, or u) from **STATION**. Your result cannot contain duplicates.

***Input Format***

The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/5abe14ff-a8ab-4ccd-a3df-6572965fad98)


where LAT_N is the northern latitude and LONG_W is the western longitude.

## Solution
```sql
SELECT DISTINCT CITY FROM STATION
WHERE CITY LIKE 'A%' OR CITY LIKE 'E%' OR CITY LIKE 'I%' OR CITY LIKE 'O%' OR CITY LIKE 'U%';
```
