### Lab Exercise 3: Using IF, AND, OR, and NOT Functions

**Objective:** Learn how to use the IF, AND, OR, and NOT functions to perform conditional data analysis.

**Instructions:**

1. **Open a New Excel Workbook:**

   - Create a new Excel workbook for this lab.

2. **Input Data:**
   - Create the following table:

| Employee Name | Sales Amount | Target Met | Performance Bonus |
| ------------- | ------------ | ---------- | ----------------- |
| John Smith    | 15000        | Yes        |                   |
| Jane Doe      | 12000        | No         |                   |
| Alice Brown   | 18000        | Yes        |                   |
| Bob Johnson   | 9000         | No         |                   |
| Carol White   | 20000        | Yes        |                   |

3. **Calculate Performance Bonus:**

   - Use the IF and AND functions to calculate the performance bonus. If the Sales Amount is greater than or equal to 15000 and the Target Met is "Yes," the bonus is 500. Otherwise, the bonus is 0.
   - **Formula in cell D2:** `=IF(AND(B2>=15000, C2="Yes"), 500, 0)`
   - Drag down to fill for all employees.

4. **Identify High Performers:**
   - Use the IF and OR functions to identify high performers. If the Sales Amount is greater than 18000 or the Target Met is "Yes," mark as "High Performer." Otherwise, mark as "Standard Performer."
   - **Formula in cell E2:** `=IF(OR(B2>18000, C2="Yes"), "High Performer", "Standard Performer")`
   - Drag down to fill for all employees.

### Example Data in Excel:

| Employee Name | Sales Amount | Target Met | Performance Bonus                     | High Performer                                                      |
| ------------- | ------------ | ---------- | ------------------------------------- | ------------------------------------------------------------------- |
| John Smith    | 15000        | Yes        | =IF(AND(B2>=15000, C2="Yes"), 500, 0) | =IF(OR(B2>18000, C2="Yes"), "High Performer", "Standard Performer") |
| Jane Doe      | 12000        | No         | =IF(AND(B2>=15000, C2="Yes"), 500, 0) | =IF(OR(B2>18000, C2="Yes"), "High Performer", "Standard Performer") |
| Alice Brown   | 18000        | Yes        | =IF(AND(B2>=15000, C2="Yes"), 500, 0) | =IF(OR(B2>18000, C2="Yes"), "High Performer", "Standard Performer") |
| Bob Johnson   | 9000         | No         | =IF(AND(B2>=15000, C2="Yes"), 500, 0) | =IF(OR(B2>18000, C2="Yes"), "High Performer", "Standard Performer") |
| Carol White   | 20000        | Yes        | =IF(AND(B2>=15000, C2="Yes"), 500, 0) | =IF(OR(B2>18000, C2="Yes"), "High Performer", "Standard Performer") |
