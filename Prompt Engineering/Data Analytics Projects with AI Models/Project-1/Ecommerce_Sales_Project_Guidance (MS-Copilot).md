# 🔰 MS-Copilot Hands-on Practice Note for the Attached Excel Workbook "Ecommerce_Sales_Data.xlsx"

---

# ✅ 1. Workbook Overview

This hands-on is based on the attached **"Ecommerce_Sales_Data.xlsx"** workbook.

The workbook contains a single transactional sales dataset that can be used for:

- ✔️ data cleaning
- ✔️ formatting and conditional formatting
- ✔️ blank-cell detection
- ✔️ duplicate removal
- ✔️ sales dashboard creation
- ✔️ city-wise and product-wise sales analysis
- ✔️ dashboard storytelling with explanatory notes

## ✳️ Sheet structure

The workbook currently contains **1 worksheet**:

- ✔️ `Ecommerce_Sales`

## ✳️ Dataset size

- ✔️ **Total data rows:** 4,620
- ✔️ **Total columns:** 12

## ✳️ Columns present in `Ecommerce_Sales`

- ✔️ 01 `OrderID` — Stores the unique identification number for each customer order.
- ✔️ 02 `CustomerName` — Captures the name of the customer who placed the order.
- ✔️ 03 `Email` — Stores the customer’s email address for communication and order updates.
- ✔️ 04 `Product` — Indicates the name of the item purchased by the customer.
- ✔️ 05 `Category` — Shows the product group or type to which the item belongs.
- ✔️ 06 `Price` — Records the selling price of one unit of the product.
- ✔️ 07 `Quantity` — Represents the number of units ordered by the customer.
- ✔️ 08 `OrderDate` — Stores the date on which the order was placed.
- ✔️ 09 `City` — Indicates the city from where the order was placed or delivered.
- ✔️ 10 `Country` — Shows the country associated with the customer or order location.
- ✔️ 11 `PaymentMethod` — Records the mode of payment used for the transaction.
- ✔️ 12 `OrderStatus` — Shows the current status of the order, such as Delivered, Pending, or Cancelled.

## ✳️ Data characteristics observed from the workbook

- ✔️ It is a single-sheet ecommerce sales dataset.
- ✔️ `OrderDate` is stored as Excel serial date values and spans **2023-01-01 to 2025-12-31**.
- ✔️ There are **10 blank cells** across the dataset.
- ✔️ There are **10 rows containing at least one blank cell**.
- ✔️ There are **no exact duplicate rows** in the current dataset.
- ✔️ Most records belong to **India**, with one blank country value.
- ✔️ The most common order status is **Delivered**.
- ✔️ The highest sales city is **Delhi**.
- ✔️ The top-performing product by sales value is **Smart Watch**.

---

# ✅ 2. Workbook Sheet Inventory

| Worksheet | Rows | Columns | Key Fields | Suggested Use in Practice |
|---|---:|---:|---|---|
| Ecommerce_Sales | 4,621 including header | 12 | OrderID, Product, Price, Quantity, OrderDate, City, PaymentMethod, OrderStatus | Cleaning, formatting, dashboarding, charting, sales analysis |

> ✴️ Note: The worksheet has **4,621 total rows including the header**, which means **4,620 actual data rows**.

---

# ✅ 3. Useful Validation Checkpoints from the Current Workbook

## ✳️ Structural checkpoints

- ✔️ The workbook has **1 worksheet** named `Ecommerce_Sales`
- ✔️ The sheet has **12 columns**
- ✔️ The dataset has **4,620 data rows**

## ✳️ Data quality checkpoints

- ✔️ There are **10 blank cells** in total
- ✔️ There are **10 rows with at least one blank value**
- ✔️ Blank values appear in these columns:
  - 🔶 `Email` → 3 blanks
  - 🔶 `Price` → 3 blanks
  - 🔶 `Category` → 1 blank
  - 🔶 `City` → 1 blank
  - 🔶 `Country` → 1 blank
  - 🔶 `PaymentMethod` → 1 blank
- ✔️ There are **0 exact duplicate rows**

## ✳️ Cleaning checkpoints

- ✔️ If all rows containing any blank cell are removed, the row count should reduce from **4,620** to **4,610**
- ✔️ Since there are no exact duplicate rows, duplicate removal should not reduce the count further unless Copilot applies a different duplicate rule

## ✳️ Business insight checkpoints

- ✔️ **Top city by sales:** Delhi
- ✔️ **Top product by sales:** Smart Watch
- ✔️ **Top category by sales:** Electronics
- ✔️ **Most frequent order status:** Delivered
- ✔️ **Most frequent payment method:** Debit Card

## ✳️ Additional summary checkpoints

- ✔️ **Total sales value** is approximately **554.78 million**
- ✔️ **Total quantity sold** is **13,964**
- ✔️ The dataset contains multiple cities and products suitable for dashboarding

---

# ✅ 4. How to Use These Prompts with MS-Copilot in Excel

- ✔️ Open the workbook **"Ecommerce_Sales_Data.xlsx"** in **Microsoft Excel**
- ✔️ Make the Auto-Save option enabled to save the file on MS-OneDrive
- ✔️ Open **Copilot in Excel**
- ✔️ Use **one prompt at a time**
- ✔️ Review the output after each task
- ✔️ Save the workbook with a new name after each completed exercise
- ✔️ Where needed, ask Copilot to create a **new worksheet**, **summary sheet**, or **dashboard sheet**
- ✔️ For class demonstration, save the updated workbook manually as a new `.xlsx` file after Copilot completes the task

---

# ✅ 5. Issue the Following Prompts in MS-Copilot to Get the Required Outcomes

---

☑️ 01. **General information:** <br>
🔴 **Prompt -**  ```We shall work on this open MS-Excel workbook "Ecommerce_Sales_Data.xlsx". Read it carefully and share details about this workbook, including worksheet name, key columns, row count, data quality issues, and what analysis can be performed on it.``` <br>

---

☑️ 02. **Data Cleaning, Formatting, and Conditional Formatting:** <br>
🔴 **Prompt -** ```Clean the whole data in the "Ecommerce_Sales" worksheet and do the necessary formatting and conditional formatting. Highlight all blank cells clearly, improve the header formatting, adjust column widths, and format numeric and date columns properly.``` <br>

---

☑️ 03. **Remove Blank Rows and Duplicate Rows:** <br>
🔴 **Prompt -** ```From the "Ecommerce_Sales" worksheet, remove all rows that contain any blank cell in any column. Then remove all duplicate rows from the dataset. Keep the cleaned data neatly formatted and easy to review.``` <br>

---

☑️ 04. **Sales Dashboard with City-wise and Product-wise Charts:** <br>
🔴 **Prompt -** ```Create a sales dashboard from the "Ecommerce_Sales" worksheet with city-wise and product-wise sales charts. Use total sales value for the analysis, create a new dashboard worksheet, and arrange the charts neatly.``` <br>

---

☑️ 05. **Complete Dashboard with Explanatory Notes:** <br>
🔴 **Prompt -** ```Using the charts and sales data from the "Ecommerce_Sales" worksheet, prepare a complete dashboard with explanatory notes. It should look like a real dashboard with KPI blocks, chart titles, summary insights, and a clean presentation layout.``` <br>

---
