# Experiment 2: DDL Commands

## AIM
To study and implement DDL commands and different types of constraints.

## THEORY

### 1. CREATE
Used to create a new relation (table).

**Syntax:**
```sql
CREATE TABLE (
  field_1 data_type(size),
  field_2 data_type(size),
  ...
);
```
### 2. ALTER
Used to add, modify, drop, or rename fields in an existing relation.
(a) ADD
```sql
ALTER TABLE std ADD (Address CHAR(10));
```
(b) MODIFY
```sql
ALTER TABLE relation_name MODIFY (field_1 new_data_type(size));
```
(c) DROP
```sql
ALTER TABLE relation_name DROP COLUMN field_name;
```
(d) RENAME
```sql
ALTER TABLE relation_name RENAME COLUMN old_field_name TO new_field_name;
```
### 3. DROP TABLE
Used to permanently delete the structure and data of a table.
```sql
DROP TABLE relation_name;
```
### 4. RENAME
Used to rename an existing database object.
```sql
RENAME TABLE old_relation_name TO new_relation_name;
```
### CONSTRAINTS
Constraints are used to specify rules for the data in a table. If there is any violation between the constraint and the data action, the action is aborted by the constraint. It can be specified when the table is created (using CREATE TABLE) or after it is created (using ALTER TABLE).
### 1. NOT NULL
When a column is defined as NOT NULL, it becomes mandatory to enter a value in that column.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) NOT NULL
);
```
### 2. UNIQUE
Ensures that values in a column are unique.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) UNIQUE
);
```
### 3. CHECK
Specifies a condition that each row must satisfy.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) CHECK (logical_expression)
);
```
### 4. PRIMARY KEY
Used to uniquely identify each record in a table.
Properties:
Must contain unique values.
Cannot be null.
Should contain minimal fields.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size) PRIMARY KEY
);
```
### 5. FOREIGN KEY
Used to reference the primary key of another table.
Syntax:
```sql
CREATE TABLE Table_Name (
  column_name data_type(size),
  FOREIGN KEY (column_name) REFERENCES other_table(column)
);
```
### 6. DEFAULT
Used to insert a default value into a column if no value is specified.

Syntax:
```sql
CREATE TABLE Table_Name (
  col_name1 data_type,
  col_name2 data_type,
  col_name3 data_type DEFAULT 'default_value'
);
```

**Question 1**


<img width="747" height="284" alt="image" src="https://github.com/user-attachments/assets/5452a861-cf5d-4ef1-bf73-713a91abd562" />


**OUTPUT**


<img width="828" height="652" alt="image" src="https://github.com/user-attachments/assets/82f4edbc-e582-4587-9103-8a4cf23a7ff2" />

**Question 2**


<img width="1096" height="602" alt="image" src="https://github.com/user-attachments/assets/a7251f0c-ea9d-4f1f-8cec-38845e4ff6a4" />



**Output:**

<img width="1218" height="623" alt="image" src="https://github.com/user-attachments/assets/7be502ff-e5fc-4a69-9d82-d13c4a21c793" />



**Question 3**


<img width="699" height="304" alt="image" src="https://github.com/user-attachments/assets/749f8d95-ac55-4a4e-9fef-783563dd6445" />



**Output:**

<img width="1068" height="594" alt="image" src="https://github.com/user-attachments/assets/6f12548b-09a6-40ee-82a2-b16a94e57cc2" />


**Question 4**

<img width="1233" height="303" alt="image" src="https://github.com/user-attachments/assets/3db86b45-d8f9-4bc2-8e1e-302645e6457c" />


**Output:**


<img width="1106" height="552" alt="image" src="https://github.com/user-attachments/assets/611e9320-5328-44ec-93cd-ef9fc6a4d691" />



**Question 5**


<img width="1060" height="313" alt="image" src="https://github.com/user-attachments/assets/78b906cd-5cd2-425c-bafd-774ddce010a6" />



**Output:**


<img width="1123" height="568" alt="image" src="https://github.com/user-attachments/assets/1b325997-d06f-4d62-ad07-ef614731d3cd" />



**Question 6**


<img width="959" height="253" alt="image" src="https://github.com/user-attachments/assets/c9d8aec1-3993-44b2-bb85-eede97ca77fb" />



**Output:**


<img width="1152" height="410" alt="image" src="https://github.com/user-attachments/assets/666c21bc-b162-4615-b73f-63e45515430a" />



**Question 7**

<img width="986" height="227" alt="image" src="https://github.com/user-attachments/assets/707f4659-400e-448a-85ba-39247fa52efc" />



**Output:**


<img width="1288" height="555" alt="image" src="https://github.com/user-attachments/assets/3fcb4601-cff4-4344-af4d-219a8433ce3d" />



**Question 8**


<img width="523" height="225" alt="image" src="https://github.com/user-attachments/assets/4d585749-a6c2-461a-9baf-af281e3c9438" />



**Output:**


<img width="812" height="559" alt="image" src="https://github.com/user-attachments/assets/73960af6-439b-4def-bf37-dc8c47a7b8ae" />



**Question 9**

<img width="626" height="229" alt="image" src="https://github.com/user-attachments/assets/092d2537-67ae-4ff3-8b91-b46470d8dff2" />



**Output:**

<img width="992" height="543" alt="image" src="https://github.com/user-attachments/assets/735c1849-121b-4387-bd4d-8d0884540a65" />



**Question 10**

<img width="631" height="268" alt="image" src="https://github.com/user-attachments/assets/f78d844d-39dc-4af5-95b8-f69f94ef84f8" />


**Output:**


<img width="1263" height="613" alt="image" src="https://github.com/user-attachments/assets/e8b5fb1a-3e15-482c-ae33-9fe630ae5df7" />




## RESULT
Thus, the SQL queries to implement different types of constraints and DDL commands have been executed successfully.
