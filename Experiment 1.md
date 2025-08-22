Experiment No: 1
1. Create the DEPT table based on the DEPARTMENT following the table instance chart
below. Confirm that the table is created.
CREATE TABLE DEPARTMENT(
DEPT_ID INTEGER(6) NOT NULL,
DEPT_NAME VARCHAR(20) NOT NULL,
MANAGER_ID INTEGER(6),
LOCATION INTEGER(4) );
ALTER TABLE DEPARTMENT
MODIFY DEPT_ID INTEGER(7);
| MANAGER_ID | int         | YES  |     | NULL    |       |
| LOCATION   | int         | YES  |     | NULL    |       |

![1](https://github.com/user-attachments/assets/bfce35cd-c883-495b-acbe-83b0132b645e)


2. Create the EMP table based on the following instance chart. Confirm that the table is
 CREATE TABLE EMP(
ID VARCHAR(6), FIRST_NAME VARCHAR(20),
LAST_NAME VARCHAR(20) NOT NULL,
DEPT_ID VARCHAR(4) );
| LAST_NAME  | varchar(20) | NO   |     | NULL    |       |
| DEPT_ID    | varchar(4)  | YES  |     | NULL    |       |

![2](https://github.com/user-attachments/assets/ec4ad900-9316-4c42-b15f-35b49fab091f)


4. Modify the EMP table to allow for longer employee last names. Confirm the
modification.(Hint: Increase the size to 50)
 ALTER TABLE EMP
 MODIFY LAST_NAME VARCHAR(50);
| LAST_NAME  | varchar(50) | YES  |     | NULL    |       |
| DEPT_ID    | varchar(4)  | YES  |     | NULL    |       |

![3](https://github.com/user-attachments/assets/4f4ae4d7-e7e5-4257-88c4-93d3c927925c)

5. Create the EMPLOYEES2 table based on the structure of EMPLOYEES table. Include
Only the Employee_id, First_name, Last_name, Salary and Dept_id coloumns. Name the columns
CREATE TABLE EMPLOYEES2(
ID INTEGER(6),
FIRST_NAME VARCHAR(20),
LAST_NAME VARCHAR(25),
SALARY INTEGER(7),
Dept_id VARCHAR(7)
); 
| SALARY     | int         | YES  |     | NULL    |       |
| Dept_id    | varchar(7)  | YES  |     | NULL    |       |

![4](https://github.com/user-attachments/assets/9eec54c9-8716-4b4b-860e-432e20f158b8)

6. Drop the EMP table.
DROP TABLE EMP;
ERROR 1146 (42S02): Table 'ltd.emp' doesn't exist
| SALARY     | int         | YES  |     | NULL    |       |
| Dept_id    | varchar(7)  | YES  |     | NULL    |       |

![5](https://github.com/user-attachments/assets/1422e5a1-d7b5-4965-b9d4-4f72212d4059)


7. Drop the First_name column from the EMP table and confirm it.
ALTER TABLE EMP
 DROP ID;
| SALARY     | int         | YES  |     | NULL    |       |
| Dept_id    | varchar(7)  | YES  |     | NULL    |       |

![6](https://github.com/user-attachments/assets/265924c2-da92-4b3a-b4c7-d70de5940654)
