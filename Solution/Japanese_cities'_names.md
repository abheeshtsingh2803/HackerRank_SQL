# Day #06 - Japanese Cities` Names
## Problem

Query the names of all the Japanese cities in the **CITY** table. The **COUNTRYCODE** for Japan is **JPN**.
The **CITY** table is described as follows:

![1449729804-f21d187d0f-CITY](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/96753dd8-1ab9-49fa-ae16-a9e1d5a7bb44)

## Solution
```sql
SELECT NAME FROM CITY
WHERE COUNTRYCODE='JPN';
```
