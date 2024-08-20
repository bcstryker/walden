### Lab Exercise 8: Creating an Amortization Table

**Objective:** Learn how to create an amortization table that shows the breakdown of each monthly payment into principal and interest over a 5-year term, using multiple sheets in Excel.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Create the "Loan Details" Sheet:**
   - Rename the first sheet to "Loan Details".
   - Enter the following loan details into your "Loan Details" sheet:

| Loan   | Principal | Term (Years) | Annual Interest Rate |
| ------ | --------- | ------------ | -------------------- |
| Loan 1 | 50000     | 5            | 5%                   |

3. **Create the "Amortization Table" Sheet:**
   - Add a new sheet and rename it to "Amortization Table".
   - Set up the amortization table headers in the "Amortization Table" sheet:

| Period | Payment | Principal Paid | Interest Paid | Remaining Balance |
| ------ | ------- | -------------- | ------------- | ----------------- |

4. **Calculate Monthly Payment:**

   - In the "Loan Details" sheet, calculate the monthly payment using the PMT function.
   - **Formula in cell B5 (or any cell you choose):** `=PMT(D2/12, C2*12, -B2)`

5. **Link Monthly Payment to "Amortization Table" Sheet:**

   - In the "Amortization Table" sheet, reference the monthly payment from the "Loan Details" sheet.
   - **Formula in cell B2:** `='Loan Details'!B5`

6. **Fill in the Amortization Table:**

   - In the "Amortization Table" sheet:
     - In the first row under Period, enter 1.
     - In the Payment column, reference the monthly payment from cell B2.
       - **Formula in cell B2:** `='Loan Details'!B5`
     - For Principal Paid, use the PPMT function.
       - **Formula in cell C2:** `=PPMT('Loan Details'!D2/12, A2, 'Loan Details'!C2*12, -'Loan Details'!B2)`
     - For Interest Paid, use the IPMT function.
       - **Formula in cell D2:** `=IPMT('Loan Details'!D2/12, A2, 'Loan Details'!C2*12, -'Loan Details'!B2)`
     - For Remaining Balance, subtract the principal paid from the previous remaining balance.
       - **Formula in cell E2:** `='Loan Details'!B2 + SUM(C$2:C2)`

7. **Copy Formulas Down:**
   - Copy the formulas down for all periods (1 to 60) to complete the amortization table.

### Example Data in Excel:

**Loan Details Sheet:**

| A      | B               | C                        | D                    |
| ------ | --------------- | ------------------------ | -------------------- |
| Loan   | Principal       | Term (Years)             | Annual Interest Rate |
| Loan 1 | 50000           | 5                        | 5%                   |
|        |                 |                          |                      |
|        | Monthly Payment | =PMT(D2/12, C2\*12, -B2) |                      |

**Amortization Table Sheet:**

| Period | Payment            | Principal Paid                                                             | Interest Paid                                                              | Remaining Balance               |
| ------ | ------------------ | -------------------------------------------------------------------------- | -------------------------------------------------------------------------- | ------------------------------- |
| 1      | ='Loan Details'!B5 | =PPMT('Loan Details'!D2/12, A2, 'Loan Details'!C2\*12, -'Loan Details'!B2) | =IPMT('Loan Details'!D2/12, A2, 'Loan Details'!C2\*12, -'Loan Details'!B2) | 'Loan Details'!B2 + SUM(C$2:C2) |
| 2      | ='Loan Details'!B5 | =PPMT('Loan Details'!D2/12, A3, 'Loan Details'!C2\*12, -'Loan Details'!B2) | =IPMT('Loan Details'!D2/12, A3, 'Loan Details'!C2\*12, -'Loan Details'!B2) | E2 - C3                         |
| 3      | ='Loan Details'!B5 | =PPMT('Loan Details'!D2/12, A4, 'Loan Details'!C2\*12, -'Loan Details'!B2) | =IPMT('Loan Details'!D2/12, A4, 'Loan Details'!C2\*12, -'Loan Details'!B2) | E3 - C4                         |
| ...    | ...                | ...                                                                        | ...                                                                        | ...                             |
