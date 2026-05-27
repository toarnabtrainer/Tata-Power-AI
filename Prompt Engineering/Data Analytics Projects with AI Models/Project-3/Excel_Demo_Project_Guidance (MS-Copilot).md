# 🔰 MS-Copilot Hands-on Practice Note for the Attached Excel Workbook "Excel_Demo.xlsx"

---

# ✅ 1. Workbook Overview

This hands-on is based on the attached **"Excel_Demo.xlsx"** workbook. The file contains operational data for:

* ✔️ email communication
* ✔️ data cleaning
* ✔️ payroll
* ✔️ banking and reconciliation
* ✔️ expenses
* ✔️ inventory
* ✔️ client follow-up
* ✔️ budget tracking
* ✔️ sales analysis

## ✳️ Total worksheets in the attached workbook

* ✔️ **11 worksheets**

## ✳️ Operational sheets used for practice

* ✔️ 01. `Formula` — Used to practice Excel formulas, calculations, and function-based data analysis.
* ✔️ 02. `Email_Data` — Used to practice generating emails, reminders, and follow-up communication from structured data.
* ✔️ 03. `Raw_Messy_Data` — Used to practice data cleaning, formatting, standardization, and duplicate removal.
* ✔️ 04. `Payroll_Data` — Used to practice salary calculation, payroll formulas, and department-wise payroll summaries.
* ✔️ 05. `Bank_Books` — Used to practice recording book-side financial transactions and reconciliation analysis.
* ✔️ 06. `Bank_Statement` — Used to practice comparing bank-side transactions with internal books for reconciliation.
* ✔️ 07. `Expenses` — Used to practice expense tracking, category-wise analysis, and monthly expense reporting.
* ✔️ 08. `Inventory` — Used to practice stock monitoring, low-stock alerts, and inventory summary preparation.
* ✔️ 09. `Client_Followup` — Used to practice follow-up tracking, sales pipeline monitoring, and client status analysis.
* ✔️ 10. `Budget_vs_Actual` — Used to practice budget comparison, variance analysis, and overspending identification.
* ✔️ 11. `Sales_Data` — Used to practice sales analysis, pivot reporting, dashboards, and business insights generation.

---

# ✅ 2. Workbook Sheet Inventory

| Worksheet | Rows | Columns | Key Fields | Suggested Use in Practice |
| ---------- | ---: | ------: | ---------- | ------------------------- |
| 01. Formula | 17 | 13 | OrderID, Product, Price, Quantity | Formula lookup/demo sheet |
| 02. Email_Data | 41 | 6 | Client_Name, Email, Course, Fee_Status | Email generation and follow-up |
| 03. Raw_Messy_Data | 45 | 3 | Name, City, Sales | Cleaning and deduplication |
| 04. Payroll_Data | 41 | 6 | Department, Basic_Salary, Bonus, Deductions | Salary formula and summaries |
| 05. Bank_Books | 41 | 3 | Date, Description, Amount | Bank reconciliation |
| 06. Bank_Statement | 41 | 3 | Date, Description, Amount | Bank reconciliation |
| 07. Expenses | 41 | 4 | Date, Category, Amount | Expense summaries and monthly reporting |
| 08. Inventory | 41 | 5 | Item_Name, Stock_Available, Reorder_Level | Low stock identification |
| 09. Client_Followup | 41 | 5 | Status, Next_Followup | Pipeline and follow-up tracking |
| 10. Budget_vs_Actual | 7 | 3 | Department, Budget, Actual | Variance analysis |
| 11. Sales_Data | 401 | 4 | Date, Region, Product, Sales_Amount | Dashboard, pivot, insights |

---

# ✅ 3. Useful Validation Checkpoints from the Current Workbook

* ✔️ `Email_Data` contains **40 client records**
  * 🔶 **20 Pending**
  * 🔶 **20 Paid**

* ✔️ **Advanced Excel** appears **8 times** in `Email_Data`

* ✔️ `Raw_Messy_Data` has **44 data rows before cleaning**
  * 🔶 after trimming and deduplication, it reduces to **40 rows**

* ✔️ `Payroll_Data` contains **40 employees** across **6 departments**

* ✔️ `Inventory` contains **40 items**
  * 🔶 **11 items** are below reorder level

* ✔️ `Budget_vs_Actual` shows **2 departments over budget**
  * 🔶 **IT**
  * 🔶 **Admin**

* ✔️ `Expenses` data spans:
  * 🔶 **January 2026**
  * 🔶 **February 2026**

* ✔️ The highest overall spend category in `Expenses` is **Travel**

* ✔️ `Sales_Data` contains **400 sales rows**
  * 🔶 top region: **West**
  * 🔶 top product: **Tally Course**

---

# ✅ 4. How to Use These Prompts with MS-Copilot in Excel

* ✔️ Open the workbook **"Excel_Demo.xlsx"** in **Microsoft Excel**
* ✔️ Make the Auto-Save option enabled to save the file on MS-OneDrive
* ✔️ Open **Copilot in Excel**
* ✔️ Use **one prompt at a time**
* ✔️ Review the changes after each task
* ✔️ Save the workbook with a new name after completing each activity
* ✔️ Where needed, ask Copilot to create a **new worksheet**, **new column**, **summary report**, or **dashboard sheet**
* ✔️ For downloadable outcome in class demonstration, save the updated workbook manually as a new `.xlsx` file

---

# ✅ 5. Issue the Following Prompts in MS-Copilot to Get the Required Outcomes

---

☑️ 01. **General information:**  <br>
🔴 **Prompt -**  ```We shall work on this open MS-Excel workbook "Excel_Demo.xlsx". Read it carefully and share details about this workbook, including worksheet names, key columns, and what each worksheet can be used for.``` <br>

---

☑️ 02. **Index_Sheet (Index Sheet Navigation):** <br>
🔴 **Prompt -** ```Create a new worksheet named "Index" in this workbook and add hyperlinks for all worksheets so that I can navigate easily. Format the sheet neatly and keep it as the first worksheet.``` <br>

---

☑️ 03. **Formula (Formula for Data Retrieval):** <br>
🔴 **Prompt -** ```In "Formula" worksheet we have master data in the range A1:G17 and secondary table in the range J1:M10. Generate suitable formulas to fill up columns K, L, M in the secondary table.``` <br>

---

☑️ 04. **Email_Data (Email Generation from Excel Data):** <br>
🔴 **Prompt -** ```Using the "Email_Data" worksheet, generate personalized payment reminder emails for clients whose fee status is Pending and payment confirmation emails for clients whose fee status is Paid. Insert separate new columns for the generated email subject and email body. Apply suitable conditional formatting for Paid and Pending records.``` <br>

---

☑️ 05. **Email_Data (Follow-up Email Automation):** <br>
🔴 **Prompt -** ```Using the "Email_Data" worksheet, draft follow-up emails for students enrolled in the Advanced Excel course. Insert a separate new column for these follow-up emails and apply suitable conditional formatting to highlight those students.``` <br>

---

☑️ 06. **Raw_Messy_Data (Data Cleaning):** <br>
🔴 **Prompt -** ```Clean the "Raw_Messy_Data" worksheet by removing extra spaces, standardizing city names, and removing duplicate records. Keep the cleaned data properly formatted and easy to review.``` <br>

---

☑️ 07. **Payroll_Data (Salary Calculation):** <br>
🔴 **Prompt -** ```Using the "Payroll_Data" worksheet, create a new column for Net Salary and use a formula to calculate it as Basic Salary + Bonus - Deductions. Apply suitable conditional formatting to highlight higher and lower salary values.``` <br>

---

☑️ 08. **Payroll_Data (Payroll Summary):** <br>
🔴 **Prompt -** ```Create a new worksheet showing a department-wise payroll summary based on the "Payroll_Data" worksheet. Include employee count and payroll totals and apply suitable conditional formatting.``` <br>

---

☑️ 09. **Bank_Books & Bank_Statement (Bank Reconciliation):** <br>
🔴 **Prompt -** ```Compare the "Bank_Books" and "Bank_Statement" worksheets and identify unmatched transactions. Mark them clearly and apply suitable conditional formatting to highlight mismatches.``` <br>

---

☑️ 10. **Bank_Books & Bank_Statement (Reconciliation Report):** <br>
🔴 **Prompt -** ```Prepare a reconciliation report in a new worksheet showing missing entries between "Bank_Books" and "Bank_Statement". Clearly separate missing entries from both sides and apply suitable conditional formatting.``` <br>

---

☑️ 11. **Expenses (Expense Analysis):** <br>
🔴 **Prompt -** ```Create a category-wise expense summary from the "Expenses" worksheet in a new worksheet. Apply suitable conditional formatting and highlight the highest expense category.``` <br>

---

☑️ 12. **Expenses (Monthly Expense Report):** <br>
🔴 **Prompt -** ```Generate a monthly expense report from the "Expenses" worksheet and identify the highest expense category. Present the result in a clean summary sheet with suitable conditional formatting.``` <br>

---

☑️ 13. **Inventory (Low Stock Alert):** <br>
🔴 **Prompt -** ```From the "Inventory" worksheet, identify items where Stock Available is below the Reorder Level. Add a new status column such as Low Stock or OK, and apply suitable conditional formatting.``` <br>

---

☑️ 14. **Inventory (Inventory Summary):** <br>
🔴 **Prompt -** ```Create a summary report of total items and low-stock items from the "Inventory" worksheet. Present the summary in a new worksheet and apply suitable conditional formatting.``` <br>

---

☑️ 15. **Client_Followup (Follow-up Tracker):** <br>
🔴 **Prompt -** ```From the "Client_Followup" worksheet, identify clients who need follow-up in the next 7 days. Add a follow-up status column and apply suitable conditional formatting to highlight them.``` <br>

---

☑️ 16. **Client_Followup (Sales Pipeline Insight):** <br>
🔴 **Prompt -** ```Create a summary of client status such as Interested, Negotiation, Closed, Follow-up, and Demo Given from the "Client_Followup" worksheet. Present it in a new worksheet with suitable conditional formatting.``` <br>

---

☑️ 17. **Budget_vs_Actual (Variance Analysis):** <br>
🔴 **Prompt -** ```Analyze the "Budget_vs_Actual" worksheet and create a variance column using Actual - Budget. Identify which departments exceeded their budget and apply suitable conditional formatting.``` <br>

---

☑️ 18. **Budget_vs_Actual (Budget Report):** <br>
🔴 **Prompt -** ```Create a report showing Budget, Actual, Variance, and Variance Percentage for each department from the "Budget_vs_Actual" worksheet. Present it neatly and apply suitable conditional formatting.``` <br>

---

☑️ 19. **Sales_Data (Sales Dashboard):** <br>
🔴 **Prompt -** ```Using the "Sales_Data" worksheet, create a sales dashboard with region-wise and product-wise charts. Arrange the dashboard neatly in a new worksheet and highlight key metrics clearly.``` <br>

---

☑️ 20. **Sales_Data (Pivot Analysis):** <br>
🔴 **Prompt -** ```Generate a pivot-style summary showing total sales by Region and Product from the "Sales_Data" worksheet. Present the summary in a new worksheet and apply suitable conditional formatting.``` <br>

---

☑️ 21. **Sales_Data (Sales Insights):** <br>
🔴 **Prompt -** ```Analyze the "Sales_Data" worksheet and identify the top-performing product and top-performing region based on total sales. Present the results in a summary sheet with suitable highlighting.``` <br>

---
