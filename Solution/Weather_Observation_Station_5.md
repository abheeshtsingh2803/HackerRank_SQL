# Day #11 - Weather Observation Station 5
## Problem

Query the two cities in **STATION** with the shortest and longest **CITY** names, as well as their respective lengths (i.e.: number of characters in the name). If there is more than one smallest or largest city, choose the one that comes first when ordered alphabetically.

The **STATION** table is described as follows:

![1449345840-5f0a551030-Station](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/56130044-b102-4d70-be98-0d729fbf403c)


where **LAT_N** is the northern latitude and **LONG_W** is the western longitude.

***Sample Input***

For example, **CITY** has four entries: **DEF, ABC, PQRS and WXY**.

***Sample Output***
```

ABC 3
PQRS 4

```
***Explanation***

When ordered alphabetically, the **CITY** names are listed as **ABC, DEF, PQRS, and WXY**, with lengths **3**, **3**, **4** and **3**. The longest name is **PQRS**, but there are **3** options for shortest named city. Choose **ABC**, because it comes first alphabetically.

**Note**
You can write two separate queries to get the desired output. It need not be a single query.

## Solution
```sql
select CITY,LENGTH(CITY) from STATION
order by Length(CITY) asc, CITY limit 1; 
select CITY,LENGTH(CITY) from STATION
order by Length(CITY) desc, CITY limit 1;
```
