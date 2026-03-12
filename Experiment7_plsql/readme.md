# Experiment 7: PL/SQL – Variables, Control Structures and Loops

## AIM
To write and execute simple PL/SQL programs using variables, loops, and conditional statements.


## THEORY

PL/SQL, which stands for Procedural Language extensions to the Structured Query Language (SQL). It is a combination of SQL along with the procedural features of programming languages.

**Syntax:**
```sql
DECLARE 
   <declarations section> 
BEGIN 
   <executable command(s)>
EXCEPTION 
   <exception handling> 
END;
```

### Basic Components of PL/SQL Block:
- DECLARE: Section to declare variables and constants.
- BEGIN: The execution section that contains PL/SQL statements.
- EXCEPTION: Handles errors or exceptions that occur in the program.
- END: Marks the end of the PL/SQL block.

# PL/SQL Programs – Steps and Expected Output

## 1. Write a PL/SQL program to find the Greatest of Two Numbers

### Steps:
- Declare two numeric variables and initialize them.
- Use an `IF` statement to compare the values.
- Display the greater number using `DBMS_OUTPUT.PUT_LINE`.

**Expected Output:**  
Greater number is: 80

### PROGRAM
```
    num1 NUMBER := 80; 
    num2 NUMBER := 50; 
BEGIN
    IF num1 > num2 THEN
        DBMS_OUTPUT.PUT_LINE('Greater number is: ' || num1);
    ELSE
        DBMS_OUTPUT.PUT_LINE('Greater number is: ' || num2);
    END IF;
END;
```

### OUTPUT

<img width="541" height="122" alt="508897988-b11a6a4a-4cbe-425d-80ce-b5d231b0f66a" src="https://github.com/user-attachments/assets/0deb23e4-f53d-450d-a70f-38061549bc37" />

---

## 2. Write a PL/SQL program to Calculate Sum of First N Natural Numbers

### Steps:
- Declare a variable `n` and assign a value (e.g., 10).
- Initialize a `sum` variable to 0.
- Use a `WHILE` loop to iterate from 1 to `n`, adding each number to the sum.
- Display the result using `DBMS_OUTPUT.PUT_LINE`.

**Expected Output:**  
Sum of first 10 natural numbers is: 55

### PROGRAM
```
SET SERVEROUTPUT ON;

DECLARE
    n NUMBER := 10;       -- Number up to which sum is calculated
    i NUMBER := 1;        -- Loop counter
    total_sum NUMBER := 0; -- To store the sum
BEGIN
    WHILE i <= n LOOP
        total_sum := total_sum + i;
        i := i + 1;
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('Sum of first ' || n || ' natural numbers is: ' || total_sum);
END;
```

### OUTPUT

<img width="617" height="163" alt="508898843-193b5266-f9a9-4632-9a9c-71ea1962d4dc" src="https://github.com/user-attachments/assets/9b631ad2-97aa-409e-8ef1-7637564134cc" />

---

## 3. Write a PL/SQL program to generate Fibonacci series

### Steps:
- Declare the variable `n` to indicate how many terms to generate.
- Initialize the first two Fibonacci numbers (0 and 1).
- Use a loop to generate the next terms using the formula `c = a + b`.
- Print each term in the series.

**Expected Output:**  
n = 7  
Fibonacci sequence: 0, 1, 1, 2, 3, 5, 8

### PROGRAM
```
DECLARE
    n NUMBER := 7;        
    a NUMBER := 0;        
    b NUMBER := 1;        
    c NUMBER;             
    i NUMBER;             
BEGIN
    DBMS_OUTPUT.PUT_LINE('Fibonacci sequence:');
    DBMS_OUTPUT.PUT(a || ', ' || b);

    FOR i IN 3..n LOOP
        c := a + b;                  
        DBMS_OUTPUT.PUT(', ' || c);  
        a := b;                      
        b := c;
    END LOOP;

    DBMS_OUTPUT.NEW_LINE;            
END;
/
```

### OUTPUT

<img width="458" height="140" alt="508900421-d9b0f411-e6b2-4eab-b7db-607fc35e1b1f" src="https://github.com/user-attachments/assets/20175807-137b-458b-8350-ef44e91b2be0" />

---

## 4. Write a PL/SQL Program to display the number in Reverse Order

### Steps:
- Declare a variable `n` and assign a value (e.g., 1535).
- Use a loop to extract each digit using modulo and reverse the number.
- Display the reversed number.

**Expected Output:**  
n = 1535  
Reversed number is 5351

### PROGRAM
```
SET SERVEROUTPUT ON;

DECLARE
    n NUMBER := 1535;       -- Original number
    original NUMBER := 1535;-- To keep the original number for display
    reversed NUMBER := 0;   -- To store the reversed number
    digit NUMBER;           -- To extract each digit
BEGIN
    WHILE n > 0 LOOP
        digit := MOD(n, 10);              -- Get the last digit
        reversed := reversed * 10 + digit;-- Build the reversed number
        n := TRUNC(n / 10);               -- Remove the last digit
    END LOOP;

    DBMS_OUTPUT.PUT_LINE('n = ' || original);
    DBMS_OUTPUT.PUT_LINE('Reversed number is ' || reversed);
END;
```

### OUTPUT

<img width="352" height="174" alt="508901770-ef0d2245-3f31-4eb4-8dda-a8fb9ab87a69" src="https://github.com/user-attachments/assets/76e00f00-3e41-4fc9-a241-dc88d951adfa" />


---

## 5. Write a PL/SQL program to find the largest of three numbers

### Steps:
- Declare three numeric variables `a`, `b`, and `c`.
- Use nested `IF-ELSIF-ELSE` conditions to find the largest among the three.
- Display the largest number.

**Expected Output:**  
a = 10, b = 9, c = 15  
Largest of three number is 15

### PROGRAM
```
SET SERVEROUTPUT ON;

DECLARE
    a NUMBER := 10;
    b NUMBER := 9;
    c NUMBER := 15;
    largest NUMBER;
BEGIN
    IF a >= b AND a >= c THEN
        largest := a;
    ELSIF b >= a AND b >= c THEN
        largest := b;
    ELSE
        largest := c;
    END IF;

    DBMS_OUTPUT.PUT_LINE('a = ' || a || ', b = ' || b || ', c = ' || c);
    DBMS_OUTPUT.PUT_LINE('Largest of three number is ' || largest);
END;
```

### OUTPUT

<img width="379" height="124" alt="508900926-b7e997e6-0b9e-451e-9985-af62a2339568" src="https://github.com/user-attachments/assets/0786ed47-f6ac-4da1-93a4-f34b802b90dd" />


## RESULT
Thus, the PL/SQL programs using variables, conditionals, and loops were executed successfully.

