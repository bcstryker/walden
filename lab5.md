### Lab Exercise 5: Basic VLOOKUP and HLOOKUP

**Objective:** Learn how to use VLOOKUP and HLOOKUP functions to find specific data in a table.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Input Data:**
   - Create the following table:

| Employee ID | Name        | Department | Salary |
| ----------- | ----------- | ---------- | ------ |
| 1001        | John Smith  | HR         | 50000  |
| 1002        | Jane Doe    | IT         | 60000  |
| 1003        | Alice Brown | Finance    | 70000  |
| 1004        | Bob Johnson | Marketing  | 55000  |
| 1005        | Carol White | IT         | 62000  |

3. **Use VLOOKUP to Find Salary:**

   - In a new cell, use VLOOKUP to find the salary of the employee with ID 1003.
   - **Formula:** `=VLOOKUP(1003, A2:D6, 4, FALSE)`

4. **Transpose the Table for HLOOKUP:**
   - Transpose the table so that the headers are in the first column.
   - Create the following transposed table:

| Employee ID | 1001       | 1002     | 1003        | 1004        | 1005        |
| ----------- | ---------- | -------- | ----------- | ----------- | ----------- |
| Name        | John Smith | Jane Doe | Alice Brown | Bob Johnson | Carol White |
| Department  | HR         | IT       | Finance     | Marketing   | IT          |
| Salary      | 50000      | 60000    | 70000       | 55000       | 62000       |

5. **Use HLOOKUP to Find Department:**
   - Use HLOOKUP to find the department of the employee with ID 1004.
   - **Formula:** `=HLOOKUP(1004, B1:F3, 2, FALSE)`
