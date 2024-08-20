### Lab Exercise 2: Text Manipulation

**Objective:** Learn how to use text functions to manipulate and combine text in Excel.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Input Data:**
   - Create the following table:

| First Name | Last Name | Full Name |
| ---------- | --------- | --------- |
| John       | Smith     |           |
| Jane       | Doe       |           |
| Alice      | Johnson   |           |
| Bob        | Brown     |           |
| Carol      | White     |           |

3. **Combine First and Last Names:**

   - In the Full Name column, combine the first name and last name using the CONCAT function: `=CONCAT(A2, " ", B2)`
   - Drag the formula down to fill for all names.

4. **Calculate the Length of Full Names:**
   - In a new column labeled "Name Length", calculate the length of each full name using the LEN function: `=LEN(C2)`
   - Drag the formula down to fill for all names.
