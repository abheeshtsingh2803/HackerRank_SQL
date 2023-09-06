# Revising Select Query 1
___

## Problem

Query all columns for all American cities in the **CITY** table with populations larger than **100000**. The **CountryCode** for America is **USA**.

The **CITY** table is described as follows:

| Field | Type |
|--|--|
| ID | NUMBER |
| NAME | VARCHAR(20) |
| COUNTRYCODE | VARCHAR(20) |
| DISTRICT | VARCHAR(20) |
| POPULATION | NUMBER |

___
## Solution

```sql
SELECT * FROM CITY WHERE COUNTRYCODE = "USA" AND POPULATION > 100000;
```
