# Day #19 - Higher Than 75 Marks
## Problem

Query the Name of any student in STUDENTS who scored higher than 75 Marks. Order your output by the last three characters of each name. If two or more students both have names ending in the same last three characters (i.e.: Bobby, Robby, etc.), secondary sort them by ascending ID.

***Input Format***

The STUDENTS table is described as follows:  

![1443815243-94b941f556-1](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/bcdf0dd1-58b0-4a8a-8389-0da1296a2bf7)

The Name column only contains uppercase (A-Z) and lowercase (a-z) letters.


***Sample Input***

![1443815209-cf4b260993-2](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/065ca4b2-a4f0-4156-9a9a-be035f45f33e)


***Sample Output***
```

Ashley
Julia
Belvet

```
***Explanation***

Only Ashley, Julia, and Belvet have Marks > 75. If you look at the last three characters of each of their names, there are no duplicates and 'ley' < 'lia' < 'vet'.

## Solution
```sql
SELECT NAME FROM STUDENTS WHERE MARKS > 75 ORDER BY RIGHT(NAME,3), ID ASC
```
