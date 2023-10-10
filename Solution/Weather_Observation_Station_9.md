# Day #15 - Weather Observation Station 9
## Problem

Query the list of **CITY** names from **STATION** that do not start with vowels. Your result cannot contain duplicates.

**Input Format**

The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/93b1371d-1b17-4772-bbcd-b2d64dbc404c)


where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

## Solution
```sql

SELECT distinct city FROM station 
WHERE city NOT LIKE 'A%' AND city  NOT LIKE 'E%' anAND city NOT LIKE 'I%' AND
      city NOT LIKE 'o%' AND city NOT LIKE 'U%';

```
