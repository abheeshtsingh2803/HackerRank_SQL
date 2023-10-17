# Day #17 - Weather Observation Station 11
## Problem

Query the list of **CITY** names from **STATION** that either do not start with vowels or do not end with vowels. Your result cannot contain duplicates.

***Input Format***

The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/153ce750-4e90-4f17-8c7b-0c435f4a6435)

where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

## Solution
``` sql
select distinct city from station 
where (city Not like 'A%' and city Not like 'E%' and city Not like 'I%' and
      city Not like 'o%' and city not like 'U%') OR 
      (city Not like '%A' and city Not like '%E' and city Not like '%I' and
      city Not like '%o' and city not like '%U');
```
