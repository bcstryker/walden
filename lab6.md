Certainly! Below is your revised lab exercise with the requested modifications:

### Lab Exercise 6: INDEX and MATCH for Flexible Data Retrieval

**Objective:** Learn how to use the INDEX and MATCH functions together for flexible data retrieval.

**Instructions:**

1. **Open a New Excel Workbook:**
   - Create a new Excel workbook for this lab.

2. **Input Data:**
   - Create the following two tables:

   **Table 1: Product Information** (Beginning in cell A1)

   | Product ID | Product Name | Category    |
   | ---------- | ------------ | ----------- |
   | 2001       | Laptop       | Electronics |
   | 2002       | Tablet       | Electronics |
   | 2003       | Chair        | Furniture   |
   | 2004       | Desk         | Furniture   |
   | 2005       | Monitor      | Electronics |

   **Table 2: Product Prices** (Beginning in cell A8)

   | Product ID | Price |
   | ---------- | ----- |
   | 2001       | 1000  |
   | 2002       | 600   |
   | 2003       | 150   |
   | 2004       | 300   |
   | 2005       | 200   |

3. **Add a Price Column to Table 1 Using INDEX and MATCH:**
   - In Table 1, add a new column labeled "Price" next to "Category".
   - Use the `INDEX` and `MATCH` functions to populate the "Price" column by retrieving the corresponding price from Table 2 based on the "Product ID".
   - **Formula Example (for the first row):** 
     ```excel
     =INDEX(Table2[Price], MATCH(A2, Table2[Product ID], 0))
     ```
   - Copy this formula down to fill in the prices for all products in Table 1.

4. **Use INDEX and MATCH to Find a Product's Name:**
   - In Table 2, add a new column labeled "Name" next to "Price".
   - Use the `INDEX` and `MATCH` functions to populate the "Name" column by retrieving the corresponding price from Table 1 based on the "Product ID".
   - **Formula:** 
     ```excel
     =INDEX(Table1[Product Name], MATCH([@[Product ID]], Table1[Product ID], 0))
     ```
   - Note: If there are multiple items in the "Furniture" category, this formula will return the first match.

### **Final Instructions:**
- Ensure that your tables are correctly populated and that the formulas are working as expected.
- Save your workbook with the name "Lab_Exercise_6.xlsx".
