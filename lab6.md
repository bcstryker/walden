### Lab Exercise 6: INDEX and MATCH for Flexible Data Retrieval

**Objective:** Learn how to use the INDEX and MATCH functions together for flexible data retrieval.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Input Data:**
   - Create the following table:

| Product ID | Product Name | Category    | Price |
| ---------- | ------------ | ----------- | ----- |
| 2001       | Laptop       | Electronics | 1000  |
| 2002       | Tablet       | Electronics | 600   |
| 2003       | Chair        | Furniture   | 150   |
| 2004       | Desk         | Furniture   | 300   |
| 2005       | Monitor      | Electronics | 200   |

3. **Use INDEX and MATCH to Find Price:**

   - In a new cell, use INDEX and MATCH to find the price of the product with ID 2004.
   - **Formula:** `=INDEX(D2:D6, MATCH(2004, A2:A6, 0))`

4. **Use INDEX and MATCH to Find Product Name:**
   - In a new cell, use INDEX and MATCH to find the product name of the item in the "Furniture" category.
   - **Formula:** `=INDEX(B2:B6, MATCH("Furniture", C2:C6, 0))`
