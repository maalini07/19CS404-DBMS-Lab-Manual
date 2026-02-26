# Experiment 4: Aggregate Functions, Group By and Having Clause

## AIM
To study and implement aggregate functions, GROUP BY, and HAVING clause with suitable examples.

## THEORY

### Aggregate Functions
These perform calculations on a set of values and return a single value.

- **MIN()** – Smallest value  
- **MAX()** – Largest value  
- **COUNT()** – Number of rows  
- **SUM()** – Total of values  
- **AVG()** – Average of values

**Syntax:**
```sql
SELECT AGG_FUNC(column_name) FROM table_name WHERE condition;
```
### GROUP BY
Groups records with the same values in specified columns.
**Syntax:**
```sql
SELECT column_name, AGG_FUNC(column_name)
FROM table_name
GROUP BY column_name;
```
### HAVING
Filters the grouped records based on aggregate conditions.
**Syntax:**
```sql
SELECT column_name, AGG_FUNC(column_name)
FROM table_name
GROUP BY column_name
HAVING condition;
```

**Question 1**

<img width="1040" height="647" alt="image" src="https://github.com/user-attachments/assets/d917d495-8f5f-459a-8aec-3a2138311385" />


**Output:**

<img width="717" height="990" alt="image" src="https://github.com/user-attachments/assets/d569ca69-24cb-437b-b14b-839dd2ab0d34" />


**Question 2**

<img width="513" height="476" alt="image" src="https://github.com/user-attachments/assets/4554ac63-be71-4f6a-8b16-5bdaf5bbf2be" />

**Output:**

<img width="867" height="926" alt="image" src="https://github.com/user-attachments/assets/a4aef16c-4a95-4326-876a-c8253365d8b0" />

**Question 3**

<img width="733" height="373" alt="image" src="https://github.com/user-attachments/assets/b27766e0-f262-4911-8f8a-85b7404f824f" />

**Output:**

<img width="446" height="655" alt="image" src="https://github.com/user-attachments/assets/62384515-8380-418e-b1af-54acffe4b99c" />


**Question 4**

<img width="504" height="341" alt="image" src="https://github.com/user-attachments/assets/c3b67709-1137-4e60-93b5-64b3c27b3398" />


**Output:**

<img width="524" height="654" alt="image" src="https://github.com/user-attachments/assets/1e9709e8-c7c6-46d9-9fca-c0d4006b5407" />

**Question 5**

<img width="645" height="349" alt="image" src="https://github.com/user-attachments/assets/eb98232b-a0d1-48d3-bf0f-425e7aa962e3" />

**Output:**

<img width="433" height="654" alt="image" src="https://github.com/user-attachments/assets/cbe12ae4-f0ac-4984-899c-2615b87d627c" />

**Question 6**

<img width="703" height="381" alt="image" src="https://github.com/user-attachments/assets/bac89d25-cdfd-4b5b-abd2-640138b75ff7" />

**Output:**

<img width="411" height="654" alt="image" src="https://github.com/user-attachments/assets/3ad30496-6082-4e4a-81fe-e9540cbb36e1" />


**Question 7**

<img width="1277" height="337" alt="image" src="https://github.com/user-attachments/assets/b8e2f455-af37-4455-a893-2031f1aad0f1" />


**Output:**

<img width="531" height="672" alt="image" src="https://github.com/user-attachments/assets/5c5c6812-8006-4f68-8ae3-e7e40e7d2791" />


**Question 8**

<img width="1277" height="373" alt="image" src="https://github.com/user-attachments/assets/4e5f04ed-d9ec-44be-84b6-a7627bbafb28" />

**Output:**

<img width="605" height="705" alt="image" src="https://github.com/user-attachments/assets/ff48ff26-6e54-4020-a929-3b7deb74fa4b" />


**Question 9**

<img width="1254" height="367" alt="image" src="https://github.com/user-attachments/assets/f2489ff0-35ed-40f5-bddb-2b853c1d918a" />


**Output:**

<img width="512" height="696" alt="image" src="https://github.com/user-attachments/assets/f8abf999-9b81-484b-9de7-769c033cf8e0" />


**Question 10**

<img width="845" height="488" alt="image" src="https://github.com/user-attachments/assets/92d8177f-dea9-4109-9fd0-c3a6bc6de8e4" />



**Output:**

<img width="609" height="854" alt="image" src="https://github.com/user-attachments/assets/f6962765-ffdd-47bc-8a07-b7fadb64fd0f" />



## RESULT
Thus, the SQL queries to implement aggregate functions, GROUP BY, and HAVING clause have been executed successfully.
