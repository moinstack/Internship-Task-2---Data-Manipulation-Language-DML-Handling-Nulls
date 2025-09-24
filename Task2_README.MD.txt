Internship Task 2 - Data Manipulation Language (DML) & Handling Nulls
Objective
This task aims to provide practical experience with fundamental SQL Data Manipulation Language (DML) commands, including INSERT, UPDATE, and DELETE. It also focuses on the proper handling of NULL values, demonstrating data integrity constraints, and using basic transaction control to manage data changes.

Key Concepts
INSERT: Used to add new rows of data into a table. The script shows various ways to insert data, including providing all column values, omitting optional columns (which results in NULL or DEFAULT values), and using a SELECT statement to copy data from existing records.

UPDATE: Used to modify existing data in a table. The examples demonstrate updating a single record, updating multiple rows that meet a specific condition, updating a column to NULL, and using a CASE statement to apply different updates based on conditions.

DELETE: Used to remove one or more rows from a table. The script shows how to delete specific records or multiple records based on conditions, including deleting rows where a column has a NULL value.

NULL Values: Represents missing or unknown data in a field. You can check for them using IS NULL or IS NOT NULL. The COALESCE function can be used to replace a NULL value with a specified alternative in a query result, making the output more user-friendly.

Constraints: Rules that enforce data integrity. The NOT NULL constraint prevents a column from having a NULL value, while the DEFAULT constraint provides a default value if none is specified during insertion.

Transactions: A sequence of SQL operations treated as a single, atomic unit. You can start a transaction with BEGIN TRANSACTION, perform operations like INSERT, and then use ROLLBACK to undo all the changes made within that transaction.

ON DELETE CASCADE: A foreign key constraint that automatically deletes a record in a child table when the corresponding record in the parent table is deleted. This is demonstrated by creating a Projects table that references the Employees table.

Files
Task2_Data_Insertion_and_Nulls.sql.txt → The complete SQL script for this task, containing all DDL (Data Definition Language) and DML (Data Manipulation Language) commands.

README.md → This file, providing a detailed overview of the task's objectives and concepts.

How to Run
Open your preferred SQL database client, such as DB Fiddle or SQLiteStudio.

Copy the entire content of the Task2_Data_Insertion_and_Nulls.sql.txt file.

Execute the script. It will first create the Task2DB database, the Employees and Departments tables, and a Projects table.

The script will then demonstrate various INSERT, UPDATE, and DELETE operations, followed by a series of SELECT statements to verify the final state of the data in each table.