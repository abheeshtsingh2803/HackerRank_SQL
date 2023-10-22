# Day #20 - Employee Names
## Problem

Write a query that prints a list of employee names (i.e.: the name attribute) from the **Employee** table in alphabetical order.

***Input Format***

The **Employee** table containing employee data for a company is described as follows:

![1458557872-4396838885-ScreenShot2016-03-21at4 27 13PM](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/9b269a7b-c710-4a9e-a694-4ea923e93b35)


where employee_id is an employee's ID number, name is their name, months is the total number of months they've been working for the company, and salary is their monthly salary.

Sample Input

![1458558202-9a8721e44b-ScreenShot2016-03-21at4 32 59PM](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/ba02f48d-48cf-4611-a786-ee905a2224c3)


Sample Output
```

Angela
Bonnie
Frank
Joe
Kimberly
Lisa
Michael
Patrick
Rose
Todd

```

## Solution
```sql
SELECT name FROM Employee ORDER BY name;
```
