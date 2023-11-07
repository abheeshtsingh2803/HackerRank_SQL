# Day #22 - Type of Triangle 
## Problem

Write a query identifying the type of each record in the **TRIANGLES** table using its three side lengths. Output one of the following statements for each record in the table:

+ **Equilateral**: It's a triangle with 3 sides of equal length.
+ **Isosceles**: It's a triangle with 2 sides of equal length.
+ **Scalene**: It's a triangle with 3 sides of differing lengths.
+ **Not A Triangle**: The given values of A, B, and C don't form a triangle.

***Input Format***

The **TRIANGLES** table is described as follows:

![1443815629-ac2a843fb7-1](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/2450c721-04e1-4096-bf1b-cb46950106de)


Each row in the table denotes the lengths of each of a triangle's three sides.

***Sample Input***

![1443815827-cbfc1ca12b-2](https://github.com/abheeshtsingh2803/HackerRank_SQL/assets/131380599/b0b8af1a-7f6e-401d-9d11-0d6f66f23b94)


***Sample Output***
```

Isosceles
Equilateral
Scalene
Not A Triangle

```

***Explanation***

Values in the tuple (20, 20, 23) form an Isosceles triangle, because A = B.<br>
Values in the tuple (20, 20, 20) form an Equilateral triangle, because A = B = C. <br>
Values in the tuple (20, 21, 22) form a Scalene triangle, because A != B != C.<br>
Values in the tuple  cannot form a triangle because the combined value of sides A and B is not larger than that of side C.<br>

## Solution
```sql
SELECT CASE
WHEN A + B <= C OR A + C <= B OR B + C <= A THEN 'Not A Triangle'
WHEN A = B AND B = C THEN 'Equilateral'
WHEN A = B OR B = C OR A = C THEN 'Isosceles'
ELSE 'Scalene'
END
FROM TRIANGLES;
```
