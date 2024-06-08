# DBMS

https://www.javatpoint.com/dbms-interview-questions
    
https://takeuforward.org/interviews/must-do-questions-for-dbms-cn-os-interviews-sde-core-sheet/

https://www.geeksforgeeks.org/30-days-of-sql-from-basic-to-advanced-level/

<img width="713" alt="image" src="https://github.com/0904-mansi/DBMS/assets/81081105/00959911-dc2c-450f-adfc-5e02676f6bd3">

<img width="713" alt="Screenshot 2024-06-08 at 12 39 23 PM" src="https://github.com/0904-mansi/DBMS/assets/81081105/dbe78a2f-b0d8-4baa-bdbd-637bf9577a85">



![image](https://github.com/0904-mansi/DBMS/assets/81081105/14a2ed32-9911-4ffc-9466-7fda2fdd9732)

<img width="1261" alt="image" src="https://github.com/0904-mansi/DBMS/assets/81081105/17dc1b39-d9a2-413e-b795-ce75238ec98b">

<img width="1261" alt="image" src="https://github.com/0904-mansi/DBMS/assets/81081105/c5e79e86-5951-4e65-83be-86f54c79af36">

<img width="958" alt="image" src="https://github.com/0904-mansi/DBMS/assets/81081105/efc6f948-fffd-4651-b413-fe6e4afaa228">


https://www.youtube.com/watch?v=gG7VyRXBfdg

In summary, the main difference between "intersection" and "inner join" lies in their operations and syntax:

    "Intersection" operates on entire result sets and returns the common rows between them.
    "Inner join" operates on individual rows from two tables and returns only the rows that have matching values based on a specified join condition.

 Cross Join:
        A cross join generates a Cartesian product of rows from both tables, resulting in every combination of rows between the two tables.
        In this case, the cross join would produce 3 * 5 = 15 rows.

 Inner Join:
        An inner join returns only the rows that have matching values in both tables based on the specified condition.
        Let's say we join on ID, and there are no matching IDs between the two tables. In this case, the inner join would return an empty result set.

   Self Join:
        A self join is when a table is joined with itself. It is often used to compare rows within the same table.
        Let's consider a self join on Table 1, where we compare each row with every other row.
        The number of rows returned in a self join depends on the condition specified. If we join the table on ID, we would get 3 * (3 - 1) = 6 rows, as each row would be compared with every other row except itself.

Now, let's calculate the counts for each type of join:

    Cross Join: 15 rows
    Inner Join: 0 rows (if no matching IDs)
    Self Join (on Table 1): 6 rows

Explain different languages present in DBMS.
Following are various languages present in DBMS:

DDL(Data Definition Language):  It contains commands which are required to define the database.
E.g., CREATE, ALTER, DROP, TRUNCATE, RENAME, etc.

DML(Data Manipulation Language): It contains commands which are required to manipulate the data present in the database.
E.g., SELECT, UPDATE, INSERT, DELETE, etc.

DCL(Data Control Language):  It contains commands which are required to deal with the user permissions and controls of the database system.
E.g., GRANT and REVOKE.

TCL(Transaction Control Language):  It contains commands which are required to deal with the transaction of the database.
E.g., COMMIT, ROLLBACK, and SAVEPOINT.
