# Day #02 - Revising the Select Query II
___
## Problem
Query the **NAME** field for all American cities in the **CITY** table with populations larger than `120000`. The **CountryCode** for America is `USA`.

The **CITY** table is described as follows:

![1449729804-f21d187d0f-CITY](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/910aec7d-739f-4cf7-8db8-846c696b7320)

## Solution
```sql
SELECT name FROM city
WHERE CountryCode = "USA" AND population > 120000;
```
