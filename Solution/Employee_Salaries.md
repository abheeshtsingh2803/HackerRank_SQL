# Day #21 - Employee Salaries
## Problem

Write a query that prints a list of employee names (i.e.: the name attribute) for employees in ***Employee*** having a salary greater than $2000 per month who have been employees for less than 10 months. Sort your result by ascending employee_id.

Input Format

The ***Employee*** table containing employee data for a company is described as follows:

![1458557872-4396838885-ScreenShot2016-03-21at4 27 13PM](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/a7eced9a-4e83-4b5b-bee2-c3cb6401e437)

where employee_id is an employee's ID number, name is their name, months is the total number of months they've been working for the company, and salary is the their monthly salary.

Sample Input

![1458558612-af3da3ceb7-ScreenShot2016-03-21at4 32 59PM](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/b0645519-b4c6-4daf-8cef-2ff1ebbb6777)

Sample Output
```

Angela
Michael
Todd
Joe

```

## Solution
```sql
SELECT NAME FROM EMPLOYEE WHERE SALARY > 2000 AND MONTHS < 10 ORDER BY EMPLOYEE_ID ASC
```
