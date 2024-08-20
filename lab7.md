### Lab Exercise 7: Calculating Total Interest Paid on Loans

**Objective:** Learn how to calculate the total interest paid over the term of a loan using the PMT function in Excel.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Input Loan Data:**
   - Create the following table:

| Loan   | Principal | Term (Years) | Annual Interest Rate |
| ------ | --------- | ------------ | -------------------- |
| Loan 1 | $50,000   | 5            | 5%                   |
| Loan 2 | $75,000   | 10           | 4.5%                 |
| Loan 3 | $100,000  | 15           | 6%                   |
| Loan 4 | $125,000  | 20           | 5.5%                 |
| Loan 5 | $150,000  | 25           | 6.5%                 |

3. **Calculate Monthly Payment:**

   - In column E, label it "Monthly Payment".
   - In cell E2, enter the formula: `=PMT(D2/12, C2*12, -B2)` and drag down to fill for all loans.

4. **Calculate Total Amount Paid Over Loan Term:**

   - In column F, label it "Total Paid".
   - In cell F2, enter the formula: `=E2*C2*12` and drag down to fill for all loans.

5. **Calculate Total Interest Paid:**
   - In column G, label it "Total Interest Paid".
   - In cell G2, enter the formula: `=F2-B2` and drag down to fill for all loans.

### Example Data in Excel:

| Loan   | Principal | Term (Years) | Annual Interest Rate | Monthly Payment          | Total Paid | Total Interest Paid |
| ------ | --------- | ------------ | -------------------- | ------------------------ | ---------- | ------------------- |
| Loan 1 | 50000     | 5            | 5%                   | =PMT(D2/12, C2\*12, -B2) | =E2*C2*12  | =F2-B2              |
| Loan 2 | 75000     | 10           | 4.5%                 | =PMT(D3/12, C3\*12, -B3) | =E3*C3*12  | =F3-B3              |
| Loan 3 | 100000    | 15           | 6%                   | =PMT(D4/12, C4\*12, -B4) | =E4*C4*12  | =F4-B4              |
| Loan 4 | 125000    | 20           | 5.5%                 | =PMT(D5/12, C5\*12, -B5) | =E5*C5*12  | =F5-B5              |
| Loan 5 | 150000    | 25           | 6.5%                 | =PMT(D6/12, C6\*12, -B6) | =E6*C6*12  | =F6-B6              |
