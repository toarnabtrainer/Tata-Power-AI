# 🔰 Claude Hands-on Practice Note for the Attached Excel Workbook "Ecommerce_Sales_Data.xlsx"

---

# ✅ 1. Workbook Overview

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

# 🔰 2. Workbook Sheet Inventory

| Worksheet | Rows | Columns | Key Fields | Suggested Use in Practice |
|---|---:|---:|---|---|
| Ecommerce_Sales | 4,621 including header | 12 | OrderID, Product, Price, Quantity, OrderDate, City, PaymentMethod, OrderStatus | Cleaning, formatting, dashboarding, charting, sales analysis |

> ✴️ Note: The worksheet has **4,621 total rows including the header**, which means **4,620 actual data rows**.

---

# 🔰 3. Useful Validation Checkpoints from the Current Workbook

Use these checkpoints to verify Claude’s output.

## ✳️ Structural checkpoints

- ✔️ The workbook has **1 worksheet** named `Ecommerce_Sales`.
- ✔️ The sheet has **12 columns**.
- ✔️ The dataset has **4,620 data rows**.

## ✳️ Data quality checkpoints

- ✔️ There are **10 blank cells** in total.
- ✔️ There are **10 rows with at least one blank value**.
- ✔️ Blank values appear in these columns:
  - 🔶 `Email` → 3 blanks
  - 🔶 `Price` → 3 blanks
  - 🔶 `Category` → 1 blank
  - 🔶 `City` → 1 blank
  - 🔶 `Country` → 1 blank
  - 🔶 `PaymentMethod` → 1 blank
- ✔️ There are **0 exact duplicate rows**.

## ✳️ Cleaning checkpoints

- ✔️ If all rows containing any blank cell are removed, the row count should reduce from **4,620** to **4,610**.
- ✔️ Since there are no exact duplicate rows, duplicate removal should not reduce the count further unless the model applies a different duplicate rule.

## ✳️ Business insight checkpoints

- ✔️ **Top city by sales:** Delhi
- ✔️ **Top product by sales:** Smart Watch
- ✔️ **Top category by sales:** Electronics
- ✔️ **Most frequent order status:** Delivered
- ✔️ **Most frequent payment method:** Debit Card

## ✳️ Additional summary checkpoints

- ✔️ **Total sales value** is approximately **554.78 million**
- ✔️ **Total quantity sold** is **13,964**
- ✔️ The dataset contains multiple cities and products suitable for dashboarding.

---

# 🔰 4. Issue the Following Prompts in Claude to Get the Required Outcomes

---

☑️ 01. **General information:** <br>
🔴 **Prompt -** ```We shall work on this attached MS-Excel workbook. Read it carefully. Please share details about the attached MS-Excel workbook "Ecommerce_Sales_Data.xlsx".``` <br>

---

☑️ 02. **Data Cleaning, Formatting, and Conditional Formatting:** <br>
🔴 **Prompt -** ```Clean the whole data and do the needful formatting and conditional formatting from "Ecommerce_Sales" worksheet. Highlight all blank cells. Generate a downloadable .xlsx file as outcome.``` <br>

---

☑️ 03. **Remove Blank Rows and Duplicate Rows:** <br>
🔴 **Prompt -** ```Remove all those rows from the dataset which are containing any blank cell from "Ecommerce_Sales" worksheet. Also remove all duplicate rows. Generate a downloadable .xlsx file as outcome.``` <br>

---

☑️ 04. **Sales Dashboard with City-wise and Product-wise Charts:** <br>
🔴 **Prompt -** ```Create a sales dashboard with city wise and product wise charts from "Ecommerce_Sales" worksheet. Generate a downloadable .xlsx file as outcome.``` <br>

---

☑️ 05. **Complete Dashboard with Explanatory Notes:** <br>
🔴 **Prompt -** ```By using these charts and data, prepare a complete dashboard with explanatory notes. Remember it should look like a dashboard. Generate a downloadable .xlsx file as outcome.``` <br>

---

☑️ **When free Claude account will get exhausted then login to another Claude account and resume working with this following prompt:** <br>
🔴 **Prompt -** ```Now onwards, we shall work on this attached MS-Excel workbook "Ecommerce_Sales_Data.xlsx". Read it carefully.``` <br>

---
