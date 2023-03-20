# Day 1 to 6

 1. [Creating Database](#create)
 2. [SELECT Clause](#select)
 3. 
  FROM Clause: From which table in the database do you have to select data?
  WHERE Clause: It forms the condition based on which data have to be queried.
  DELETE Statement: For deletion tasks.
  INSERT INTO: For insertion tasks.
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
