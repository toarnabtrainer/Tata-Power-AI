## MS-Excel with MS-CoPilot

<hr>

### **1️⃣ What is MS-CoPilot for MS-Excel and How to Enable It?**
- ✅ MS-CoPilot is an AI assistant integrated into MS-Excel and also with other Office apps.
- ✅ To use it, ensure that you have the correct **Microsoft license** and that your **IT admin has assigned** you the access.
- ✅ The MS-Excel Workbook must be saved on **SharePoint or OneDrive** for MS-CoPilot to function.
- ✅ Dataset should be converted to a Table format to resist **Data Leakage** problem.

<hr>

### **2️⃣ Use of Microsoft MS-CoPilot in MS-Excel.**
- ✅ Microsoft CoPilot is an **AI-powered assistant** integrated into MS-Excel, designed to automate tasks, analyze data, and improve efficiency. Below are its key uses:
  - ### **☑️ A. Data Cleaning & Transformation**
    - 🔰 Automatically **detects patterns** and helps format data.
    - 🔰 Extracts information (e.g., "Get the day of the week from a date").
    - 🔰 Helps in **removing duplicates, filling missing data, and organizing datasets**.
  - ### **☑️ B. Writing & Explaining Formulas**
    - 🔰 Generates **complex MS-Excel formulas** based on natural language prompts.
    - 🔰 Explains existing formulas step by step (e.g., "What does this formula do?").
    - 🔰 Assists with functions like `IF`, `XLOOKUP`, `FILTER`, `VLOOKUP`, `SUMIFS`, etc.
  - ### **☑️ C. Data Analysis & Insights**
    - 🔰 Identifies **trends, anomalies, and key patterns** in datasets.
    - 🔰 Provides **natural language summaries** of data insights.
    - 🔰 Answers queries like **“Which product had the highest sales?”**.
  - ### **☑️ D. Interactive Data Filtering & Sorting**
    - 🔰 Filters data based on user queries (e.g., “Show sales above $500”).
    - 🔰 Supports **voice commands** for hands-free filtering and sorting.
  - ### **☑️ E. Creating Charts & Visualizations**
    - 🔰 Generates **pivot tables, bar charts, scatter plots**, and more.
    - 🔰 Automatically **suggests the best visualization** based on data.
  - ### **☑️ F. Revenue Forecasting & Predictive Analysis**
    - 🔰 Helps calculate future revenue based on trends and assumptions.
    - 🔰 Assists in **financial modelling and budget planning**.
  - ### **☑️ G. Pivot Table and Pivot Chart Creation**
    - 🔰 Automates the creation of **pivot tables** for summarized reporting.
    - 🔰 Provides insights based on **sales, customer trends, and performance metrics**.
  - ### **☑️ H. AI-Driven Decision Support**
    - 🔰 Helps in **what-if analysis** (e.g., “What happens if sales increase by 10%?”).
    - 🔰 Suggests strategies based on historical data patterns.
  - ### **☑️ Limitations & Considerations**
    - 🔰 Requires a **compatible Microsoft 365 license**.
    - 🔰 Needs an **active internet connection** to function.
    - 🔰 Works best when **data is structured in tables or ranges**.
    - 🔰 AI responses **may vary**, requiring manual verification.
    - 🔰 MS-CoPilot can analyze trends but sometimes **misinterprets data**, leading to misleading graphs.
    - 🔰 Formatting issues (e.g., displaying full dates instead of day names) can affect **pivot table accuracy**.
    - 🔰 AI tools struggle with **contextual understanding**, requiring manual verification.
  - ### **☑️ Alternatives to MS-CoPilot in MS-Excel**
    - 🔰 MS-Excel has built-in AI features like **Flash Fill, Power Query, and recommended charts/tables**.
    - 🔰 These tools provide additional **Automation and Data Insights** without MS-CoPilot.
  - ### **☑️ Conclusion**
    - 🔰 Users can ask MS-CoPilot in **plain English** to extract information (e.g., the day of the week from a date column).
    - 🔰 It supports **voice commands**, allowing users to interact via microphone.
    - 🔰 Microsoft CoPilot in MS-Excel is a powerful tool that enhances **productivity, automation, and decision-making** by simplifying complex tasks. While it has limitations, its ability to streamline workflows makes it a **game-changer** for professionals dealing with data analysis, financial planning, and reporting. 🚀

<hr>

#### **3️⃣ Open the MS-Excel workbook file.**
- ✅ Open the MS-Excel workbook for the required worksheet (e.g. **PE-Classwork.xlsx** ➡️ **Cookies Orders** worksheet).
- ✅ Save the workbook either on MS-OneDrive or on MS-SharePoint.
- ✅ Covert the dataset to a table to avoid data leakage problem. Give the table name as **"CookiesOrders"**.
- ✅ Open the MS-CoPilot on the right side pane.
- ✅ MS-CoPilot can auto-detect the extent of the dataset (i.e. number of rows and columns of the dataset) if we don't convert the dataset to a table.

<hr>

#### **4️⃣ Prompts for different operations on the table.**
- ✅ Issue the following prompts in sequence and observe the outputs.
  - 🔴 **Prompt (Format) -** `Format "Order Date" in the format 'dd-mmm-yyyy".`
  - 🔴 **Prompt (Filter) -** `Do the filtering on the table with "Cost" greater than 2000.`
  - 🔴 **Prompt (Undo) -** `Clear all the filters.`
  - 🔴 **Prompt (Insert Column) -** `Add a column with the calculated profit values.`
  - 🔴 **Prompt (Format) -** `Format the currency of the columns "Revenue", "Cost" and "Profit" to $.`
  - 🔴 **Prompt (Conditional Formatting) -** `Bold TOP 10 values of "Profit" column.`
  - 🔴 **Prompt (Sort) -** `Sort "Profit" in the descending order.`
  - 🔴 **Prompt (Filter) -** `Filter for the month of August.`
  - 🔴 **Prompt (Undo) -** `Clear all filters.`
  - 🔴 **Prompt (Undo) -** `Clear all Conditional Formatting.`
  - 🔴 **Prompt (Processing) -** `How many distinct "Customers Name"?`
  - 🔴 **Prompt (Conditional Formatting) -** `Can you highlight the "Profit" in Green color when above 2000?`
  - 🔴 **Prompt (Undo) -** `Clear all Conditional Formatting.`
  - 🔴 **Prompt (Insert Column) -** `Create a column by concatenating "Cookies Shipped" and "Revenue".`
  - 🔴 **Prompt (Tabular Report) -** `Which Customer ordered most number of Cookies?`
  - 🔴 **Prompt (Tabular Report) -** `Generate "Customer Name" wise total, maximum, minimum, average of "Revenue".`
  - 🔴 **Prompt (Pivot Table / Pivot Chart) -** `Can you make a Line Chart showing "Profit" against each month?`
  - 🔴 **Prompt (Visualization) -** `Are there any seasonal trend in Cookies "Revenue"?`
  - 🔴 **Prompt (Pivot Table / Pivot Chart) -** `Customer wise total "Revenue" collected.`
  - 🔴 **Prompt (Pivot Table / Pivot Chart) -** `Quarter wise total "Revenue" collected.`
  - 🔴 **Prompt (Prediction) -** `If quarter wise total "Revenue" are (Qtr1, $7,09,665.00), (Qtr2, $6,71,830.00), (Qtr3, $7,91,970.00), (Qtr4, $15,72,525.00). Using trend analysis, can you predict the total "Revenue" for the next quarter?`
  - 🔴 **Prompt (Follow Up) -** `Can you please do your suggested calculations for me and generate the value?`
  - 🔴 **Prompt (Insert Column) -** `Insert a column Age in years, months and days calculated from Order Date.`
  - 🔴 **Prompt (Data Insight) -** `Show data insight.`
  - 🔴 **Prompt (Data Insight) -** `Add all insights to grid.`

<hr>

#### **5️⃣ Tips and Tricks.**
- ✅ MS-CoPilot also gives us some helpful prompts. We can try with them.
- ✅ We can also click on the refresh button to fetch some more other helpful prompts.
- ✅ At the top of the pane, we can get some other useful guidelines as well.
- ✅ From the chat history button we can get previous issued prompts.

<hr>
