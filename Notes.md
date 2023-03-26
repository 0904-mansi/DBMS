# Day 1 to 6

 1. [create table](#create-table)
 2. [SELECT Clause](#select-clause)
 3. [WHERE Clause](#where-Clause)
 4. [DELETE Clause](#delete-clause)
 5. [INSERT](#insert)
 6. 
  AND and OR operator: Selecting data based on AND or operator.
  Drop and Truncate: It will drop or truncate the collection as per the condition.
  NOT Operator: It will select the data which is not based on the given condition.
  
  
# Create table
 ## SQL CREATE TABLE Statement

A Table is a combination of rows and columns. For creating a table we have to define the structure of a table by adding names to columns and providing data type and size of data to be stored in columns.
Syntax:
```
CREATE table table_name
(
Column1 datatype (size),
column2 datatype (size),
.
.
columnN datatype(size)
);
```

## Example
```
CREATE TABLE Subject
(
Sub_ID INT, 
Sub_Name varchar(20)
);
```

# Add data to the Table

To add data to the table, we use INSERT INTO, the syntax is as shown below:
Syntax:
```
Insert into Table_name(Column1, Column2, Column3)
Values (Value1, value2, value3);
```

## Example

```
//Adding multiple data in the table in one go//
Insert into Subject
Values (1,'English'),
(2,'French'),
(2,'Science'),
(2,'Maths');

```
# Create a Table Using Another Table

Syntax:

```
CREATE TABLE new_table_name AS
    SELECT column1, column2,...
    FROM existing_table_name
    WHERE ....;
```


# Select clause

Select is the most commonly used statement in SQL. The SELECT Statement in SQL is used to retrieve or fetch data from a database. We can fetch either the entire table or according to some specified rules. 

To fetch the entire table or all the fields in the table:
```
 SELECT * FROM table_name; 
```

Example
```
SELECT column1,column2 FROM table_name 
column1 , column2: names of the fields of the table
table_name: from where we want to apply query
```
# WHERE Clause

WHERE keyword is used for fetching filtered data in a result set. It is used to fetch data according to a particular criteria. WHERE keyword can also be used to filter data by matching patterns.

## Basic Syntax: 

```
SELECT column1,column2 FROM table_name WHERE column_name operator value;
```
![image](https://user-images.githubusercontent.com/81081105/226430500-379b9fa9-1f6d-4a43-bf47-e055dbc6be36.png)

# BETWEEN operator

It is used to fetch filtered data in a given range inclusive of two values. Basic Syntax: SELECT column1,column2 FROM table_name WHERE column_name BETWEEN value1 AND value2;

To fetch records of students where ROLL_NO is between 1 and 3 (inclusive)
```
SELECT * FROM Student WHERE ROLL_NO BETWEEN 1 AND 3;
```

# LIKE operator

It is used to fetch filtered data by searching for a particular pattern in where clause. Basic Syntax: SELECT column1,column2 FROM table_name WHERE column_name LIKE pattern;

 To fetch records of students where NAME starts with letter S.
```
SELECT * FROM Student WHERE NAME LIKE 'S%'; 
```
The ‘%'(wildcard) signifies the later characters here which can be of any length and value.More about wildcards will be discussed in the later set

# IN operator

It is used to fetch filtered data same as fetched by ‘=’ operator just the difference is that here we can specify multiple values for which we can get the result set. Basic Syntax: SELECT column1,column2 FROM table_name WHERE column_name IN (value1,value2,..);

  To fetch NAME and ADDRESS of students where Age is 18 or 20.
```
SELECT NAME,ADDRESS FROM Student WHERE Age IN (18,20);
```

# DELETE clause

The DELETE Statement in SQL is used to delete existing records from a table. We can delete a single record or multiple records depending on the condition we specify in the WHERE clause.

Syntax: Basic 

DELETE FROM table_name WHERE some_condition;

# INSERT

The INSERT INTO statement of SQL is used to insert a new row/record in a table. There are two ways of using the INSERT INTO statement for inserting rows.

`
Syntax:

    INSERT INTO table_name (column1, column2, column3) 

    VALUES ( value1, value2, value3); 
    
    or 
    
    INSERT INTO table_name VALUES (value1, value2, value3); 
    
    
`

  inserting all columns of a table: We can copy all the data of a table and insert it into a different table.

Syntax:

    INSERT INTO first_table SELECT * FROM second_table;
