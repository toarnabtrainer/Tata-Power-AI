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
- ✅ Open the MS-Excel workbook for the required worksheet (e.g. **PE-Classwork.xlsx** ➡️ **PopStar** worksheet).
- ✅ Save the workbook either on MS-OneDrive or on MS-SharePoint.
- ✅ Convert the dataset to a table to avoid data leakage problem. Give the table name as **"PopStar"**.
- ✅ Open the MS-CoPilot on the right side pane.
- ✅ MS-CoPilot can auto-detect the extent of the dataset (i.e. number of rows and columns of the dataset) if we don't convert the dataset to a table.

<hr>

#### **4️⃣ Prompts for Inserting New Columns to the table.**
- ✅ We want to extract the day of each date.
  - 🔴 **Prompt -** `Extract the day of week and print the names in the adjacent column.`
- We want to watch events only in the weekends (i.e. Friday, Saturday and Sunday).
  - 🔴 **Prompt -** `Can you add a column to tell me if this is a weekday or weekend. Assume Friday to Sunday as weekend.`
- ✅ Check MS-CoPilot has used a formula weekday() to do this.
- ✅ If you could not understand the formula weekday(), then you can ask a follow up prompt to MS-CoPilot to explain it.
  - 🔴 **Prompt -** `Can you explain me how did you do this?`

![image](https://github.com/user-attachments/assets/8eae41fa-d0e1-45d7-9024-3aa548e43845)

<hr>

#### **5️⃣ Prompts for Filtering and Formatting.**
- ✅ Let us suppose our budget is $200 and location is "San Diego". so, we want to know all the feasible events.
  - 🔴 **Prompt -** `My budget is $200 and I live in San Diego, which events can I attend in weekend only?`
- ✅ Probably we have got a line graph which was not expected but the generated text is meaningful to us.
  - 🔴 **Prompt -** `Can you filter values instead?`
- ✅ Now the filtered data is purposeful to us.
  - 🔴 **Prompt -** `Please clear all the filters.`
 
<hr>

#### **6️⃣ Prompts for Highlighting and Sorting some data.**
- ✅ Issue the following prompt.
  - 🔴 **Prompt -** `Can you highlight all the dates in the next 30 days?`
- ✅ Required conditional formatting has been imposed.
- ✅ Let us select Top 10 "Venue Size".
  - 🔴 **Prompt -** `Highlight Top 10 "Venue Size" values.`
  - 🔴 **Prompt -** `Sort "Venue Size" in the descending order.`
  - 🔴 **Prompt -** `Please clear all conditional formatting.`

<hr>

#### **7️⃣ Prompts for Complex Scenarios.**
- ✅ Let us go for some revenue forecasting.
  - 🔴 **Prompt -** `Assuming each venue is filled to 80% of its size. What would be the total money made?`
- ✅ If we don't get any proper response from MS-CoPilot, then we can issue the following prompt.
  - 🔴 **Prompt -** `Assuming each venue is filled to 80% of its size. What would be the total money made? For example, for $250 ticket price and venue size of 1,00,000, the total money would be 250 x 1,00,000 x 0.80.`
- ✅ Such prompt type is called **"One Shot Prompt"** as we are giving one example to resolve the ambiguity of the prompt.

<hr>

#### **8️⃣ Prompts for Pivot Table and Pivot Charts.**  
- ✅ Let us calculate venue wise total revenue earned.
  - 🔴 **Prompt -** `Can you generate a Pivot Table of total money made by each venue? Also generate a graph for the same.`
  - 🔴 **Rephrased Prompt -** `Can you generate a report on venue wise total money made? Also generate a graph for the same.`
  - 🔴 **Rephrased Prompt -** `Can you tell me total revenue against each venue?`
- ✅ If these prompts do not generate required pivot table and pivot chart then create a new column "Revenue".
  - 🔴 **Prompt -** `Insert a new column "Revenue" against the formula "Ticket Price" * "Venue Size".`
  - 🔴 **Prompt -** `Convert the currency of "Revenue" column to $.`
- ✅ A new column "Revenue" will be inserted and its currency type will be formatted to $.
  - 🔴 **Prompt -** `Generate total "Revenue" made by each venue.`
- ✅ Now the required Pivot Table and Pivot Chart will be created in a new worksheet.

<hr>

#### **9️⃣ Prompts for MS-CoPilot Automatic Analysis.**
- ✅ Issue the following prompt.
  - 🔴 **Prompt -** `In our present data are you finding anything interesting?`
- ✅ We can analyze the generated Pivot Table and Pivot Chart accordingly to get more insights.

<hr>

#### **🔟 Tips and Tricks.**
- ✅ MS-CoPilot also gives us some helpful prompts. We can try with them.
- ✅ We can also click on the refresh button to fetch some more other helpful prompts.
- ✅ At the top of the pane, we can get some other useful guidelines as well.
- ✅ From the chat history button we can get previous issued prompts.

<hr>
