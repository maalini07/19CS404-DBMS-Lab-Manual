# Experiment 5: Subqueries and Views

## AIM
To study and implement subqueries and views.

## THEORY

### Subqueries
A subquery is a query inside another SQL query and is embedded in:
- WHERE clause
- HAVING clause
- FROM clause

**Types:**
- **Single-row subquery**:
  Sub queries can also return more than one value. Such results should be made use along with the operators in and any.
- **Multiple-row subquery**:
  Here more than one subquery is used. These multiple sub queries are combined by means of ‘and’ & ‘or’ keywords.
- **Correlated subquery**:
  A subquery is evaluated once for the entire parent statement whereas a correlated Sub query is evaluated once per row processed by the parent statement.

**Example:**
```sql
SELECT * FROM employees
WHERE salary > (SELECT AVG(salary) FROM employees);
```
### Views
A view is a virtual table based on the result of an SQL SELECT query.
**Create View:**
```sql
CREATE VIEW view_name AS
SELECT column1, column2 FROM table_name WHERE condition;
```
**Drop View:**
```sql
DROP VIEW view_name;
```

**Question 1**

<img width="1012" height="730" alt="image" src="https://github.com/user-attachments/assets/7fc3b3f7-5348-47e5-bc75-431ccd68d518" />


**Output:**

<img width="1276" height="915" alt="image" src="https://github.com/user-attachments/assets/215c4e00-08e3-4350-bb4c-8b9ff76c73fe" />


**Question 2**

<img width="1087" height="540" alt="image" src="https://github.com/user-attachments/assets/acb5fc9c-a336-49d8-9d33-6d0ae4e0a7b7" />


**Output:**

<img width="605" height="1009" alt="image" src="https://github.com/user-attachments/assets/64539d1c-a9c2-4410-80dc-8b971a16ddc1" />


**Question 3**

<img width="951" height="734" alt="image" src="https://github.com/user-attachments/assets/4a97cd70-62fd-4584-a643-1fa7bad0c9f2" />


**Output:**

<img width="1116" height="951" alt="image" src="https://github.com/user-attachments/assets/050ecfa7-5720-4eec-998e-7346692a96fb" />


**Question 4**

<img width="1196" height="733" alt="image" src="https://github.com/user-attachments/assets/00e1dc70-638b-4a77-a855-bd9af050b8eb" />

**Output:**

<img width="1259" height="979" alt="image" src="https://github.com/user-attachments/assets/e264561f-4cdd-4415-8b55-b6f9e0932f56" />


**Question 5**

<img width="1202" height="803" alt="image" src="https://github.com/user-attachments/assets/59255d15-e7c9-47d6-9243-497311dd1aa4" />


**Output:**

<img width="1269" height="1008" alt="image" src="https://github.com/user-attachments/assets/401eb96f-48ed-4702-9187-8187d13ccf1b" />


**Question 6**

<img width="1179" height="790" alt="image" src="https://github.com/user-attachments/assets/861ccca8-ad3f-4793-873e-2a7bf606d73c" />


**Output:**

<img width="1166" height="936" alt="image" src="https://github.com/user-attachments/assets/1a03efd2-a81e-4ec2-9ca5-59d932501ad8" />


**Question 7**

<img width="961" height="615" alt="image" src="https://github.com/user-attachments/assets/503b0281-e9c9-48e7-8bd7-6925c877a4f0" />


**Output:**

<img width="1025" height="790" alt="image" src="https://github.com/user-attachments/assets/e9a81e34-daac-4e49-bb17-fdfff790669d" />


**Question 8**

<img width="876" height="593" alt="image" src="https://github.com/user-attachments/assets/c3abab83-2117-4c90-9484-95904f801571" />


**Output:**

<img width="1133" height="907" alt="image" src="https://github.com/user-attachments/assets/f2673efc-0ed7-47d9-80f8-b86fc45f92f3" />


**Question 9**

<img width="953" height="551" alt="image" src="https://github.com/user-attachments/assets/e502ee41-4956-4e03-9c78-82c0ed6d67ea" />


**Output:**

<img width="1134" height="817" alt="image" src="https://github.com/user-attachments/assets/6a5eb3db-9f95-4d1e-bca9-a56bb6688348" />


**Question 10**

<img width="1250" height="555" alt="image" src="https://github.com/user-attachments/assets/a4c55bff-4229-43c9-a378-21e0dfcc83ce" />


**Output:**

<img width="1140" height="914" alt="image" src="https://github.com/user-attachments/assets/ee509d78-2267-40b5-aae8-12a7bf203afe" />



## RESULT
Thus, the SQL queries to implement subqueries and views have been executed successfully.
