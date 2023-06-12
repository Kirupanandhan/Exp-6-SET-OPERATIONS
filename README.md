# Ex-06-SET-OPERATIONS
## AIM:-
To write a sql query to perform set operations on two tables.

## PROCEDURE:-
### STEP 1:
create database SET_OPERATION.

### STEP 2:
create table A,B.

### STEP 3:
Insert Value to the tables.

### STEP 4:
Perform Set operations like Union,Union all,Intersect,Except.

### PROGRAM:-
```sql
CREATE DATABASE SET_OPERATION;
SHOW DATABASES;
USE SET_OPERATION;
CREATE TABLE A (
  ID INT PRIMARY KEY,
  name VARCHAR(50)
);
CREATE TABLE B (
  ID INT PRIMARY KEY,
  name VARCHAR(50)
);
INSERT INTO A (ID, name) VALUES (1, 'John');
INSERT INTO A (ID, name) VALUES (2, 'Mary');
INSERT INTO A (ID, name) VALUES (3, 'David');
INSERT INTO B (ID, name) VALUES (2, 'Mary');
INSERT INTO B (ID, name) VALUES (3, 'David');
INSERT INTO B (ID, name) VALUES (4, 'Lisa');
SELECT * FROM A;

SELECT * FROM B;

SELECT * FROM A
UNION
SELECT * FROM B;

SELECT * FROM A
UNION ALL
SELECT * FROM B;

SELECT * FROM A
INTERSECT
SELECT * FROM B;

SELECT * FROM A
EXCEPT
SELECT * FROM B;
```
## OUTPUT:-
![image](https://github.com/Kirupanandhan/Exp-6-SET-OPERATIONS/assets/94386222/19e85aea-6ff9-4f66-9426-8dd5336b4a15)
<br>
![image](https://github.com/Kirupanandhan/Exp-6-SET-OPERATIONS/assets/94386222/8ebf4895-e95f-4054-9ccd-496d5689b924)<br>
![image](https://github.com/Kirupanandhan/Exp-6-SET-OPERATIONS/assets/94386222/e33f8b0c-52c8-41a1-b488-7481cb3e1f29)<br>
![image](https://github.com/Kirupanandhan/Exp-6-SET-OPERATIONS/assets/94386222/a3f8f427-48d4-4bbf-9f89-a7252f080e4d)<br>
![image](https://github.com/Kirupanandhan/Exp-6-SET-OPERATIONS/assets/94386222/036a4224-b1d4-44fb-b952-af9fb0282eac)<br>
![image](https://github.com/Kirupanandhan/Exp-6-SET-OPERATIONS/assets/94386222/f890d26d-83fa-4ade-b5a3-d709d12f63af)
## RESULT:-
A sql query to perform set operations on two tables has been executed.
