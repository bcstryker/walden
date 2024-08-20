### Lab Exercise 4: Using SUMIF and SUMIFS Functions

**Objective:** Learn how to use the SUMIF and SUMIFS functions to sum values based on single and multiple criteria.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Input Data:**
   - Create the following table:

| Region | Product | Sales Amount |
| ------ | ------- | ------------ |
| North  | A       | 10000        |
| South  | B       | 15000        |
| East   | A       | 12000        |
| West   | C       | 9000         |
| North  | B       | 14000        |
| South  | A       | 13000        |
| East   | B       | 11000        |
| West   | A       | 8000         |

3. **Calculate Total Sales for Product A:**

   - Use the SUMIF function to calculate the total sales for Product A.
   - **Formula in cell D2:** `=SUMIF(B2:B9, "A", C2:C9)`

4. **Calculate Total Sales for Each Region:**
   - Use the SUMIFS function to calculate the total sales for each region and product.
   - **Formula for North in cell D3:** `=SUMIFS(C2:C9, A2:A9, "North", B2:B9, "A")`
   - Repeat the formula for each region and product combination.

### Example Data in Excel:

| Region | Product | Sales Amount | Total Sales for Product A | Total Sales for Region and Product         |
| ------ | ------- | ------------ | ------------------------- | ------------------------------------------ |
| North  | A       | 10000        | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "North", B2:B9, "A") |
| South  | B       | 15000        | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "South", B2:B9, "B") |
| East   | A       | 12000        | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "East", B2:B9, "A")  |
| West   | C       | 9000         | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "West", B2:B9, "C")  |
| North  | B       | 14000        | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "North", B2:B9, "B") |
| South  | A       | 13000        | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "South", B2:B9, "A") |
| East   | B       | 11000        | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "East", B2:B9, "B")  |
| West   | A       | 8000         | =SUMIF(B2:B9, "A", C2:C9) | =SUMIFS(C2:C9, A2:A9, "West", B2:B9, "A")  |
