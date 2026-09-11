# Finance-Analysis-Dashboard-Power-BI

**Objective:**

**📖 What is this project about?**

This project analyzes the 2023 financial performance of a company operating across **Sports Equipment, Sportswear, and Nutrition & Food Supplements**. The Power BI dashboard focuses on:

- **Financial Performance**: Monitoring revenue, gross profit, net profit, and net profit margin to evaluate overall business performance.
- **Business Line Performance**: Comparing revenue contribution, profitability, and monthly performance across different business lines.
- **Cost Structure**: Analyzing fixed, fulfillment, and growth costs to understand cost drivers and identify areas for improving operating efficiency.

**👤 Who is this project for?**

This dashboard is designed for key stakeholders involved in financial and business performance management, including:

- **Finance Manager / CFO**: To monitor profitability, cost structure, and overall financial performance for management decision-making.
- **Business Line Managers**: To evaluate the performance and profitability of each business line and identify opportunities for growth and improvement.
- **Board of Directors (BOD)**: To gain a high-level view of revenue, profitability, and cost trends to support strategic planning and resource allocation.

**❓Business Questions:**

- How is the company performing in terms of revenue, gross profit, and net profit?
- Which business lines generate the most revenue and which are the most profitable?
- How does the performance of each business line change over time?
- What are the major cost drivers, and how are costs distributed across business lines?
- Is the company becoming more cost-intensive as fixed costs increase relative to revenue?
- Does higher revenue tend to be associated with higher profitability?
- Which business lines or cost areas require further management attention?

**🎯Project Outcome:**

The project provided a comprehensive view of **financial performance, business line profitability, and cost structure**, helping identify key performance drivers and areas requiring management attention.

#### Key Results:

- **Sports Equipment** generated the highest revenue contribution but achieved a lower net profit margin than Sportswear, indicating room for profitability improvement.
- **Sportswear** achieved the highest net profit margin, suggesting stronger profitability and potential for further growth.
- **Nutrition & Food Supplements** operated at a negative net profit margin, with a relatively high share of growth costs, particularly R&D.
- **Fulfillment Cost** was the largest cost category, accounting for more than half of total expenses and making it a key area for cost management.
- The **fixed cost-to-revenue ratio** showed an overall upward trend during 2023, highlighting the need to monitor fixed-cost expansion relative to revenue growth.
- Revenue and net profit margin showed a **positive relationship**, suggesting that higher revenue was generally associated with stronger profitability across the analyzed periods/business lines.

#### Outcome:

The analysis provided data-driven insights into **profitability, business line performance, and cost efficiency**, helping management identify priority areas for growth, cost control, and resource allocation.
## 📂 Dataset Description & Data Structure

### 📌 Data Source

- **Source:** Financial Analysis Dataset
- **Period:** January – December 2023
- **Size:** 580 records
- **Format:** Excel (.xlsx)
- **Business Lines:** Sports Equipment, Sportswear, Nutrition & Food Supplements

### 📊 Data Structure & Relationships

#### 1️⃣ Tables Used

The dashboard is built from a financial dataset containing revenue and expense transactions for three business lines throughout 2023.

The Power BI data model consists of:

- 📄 **revenue_expense** – Original dataset containing revenue and expense line items.
- 💰 **revenue** – Revenue fact table used to analyze revenue performance by business line and date.
- 💸 **expense** – Expense fact table used to analyze cost structure and profitability.
- 📅 **dim_date** – Date dimension used for time-based analysis.
- 🏷️ **dim_Business Line** – Business line dimension used to analyze and compare business line performance.

#### 2️⃣ Table: revenue_expense

The original dataset contains revenue and expense records at the **monthly business-line and financial line-item level**.

| Column Name | Description |
|---|---|
| `Year` | Year of the revenue or expense record |
| `Month - name` | Month name |
| `Month -sequence` | Month sequence |
| `Date` | Date associated with the financial record |
| `Business Line` | Business line associated with the record |
| `Amount, $` | Revenue or expense amount in USD |
| `Expense subgroup` | Detailed expense category |
| `Revenue / Expense Group` | High-level revenue or expense group |
| `Revenue or expense` | Indicates whether the record is Revenue or Expense |

#### 3️⃣ Table: revenue

The `revenue` table is derived from the original dataset and contains revenue-related records used to analyze sales performance.

| Column Name | Description |
|---|---|
| `Amount, $` | Revenue amount in USD |
| `Business Line` | Business line generating the revenue |
| `Date` | Revenue date |
| `Revenue Group` | Revenue category |

#### 4️⃣ Table: expense

The `expense` table contains expense-related records used to analyze cost structure and profitability.

| Column Name | Description |
|---|---|
| `Amount $` | Expense amount in USD |
| `Business Line` | Business line associated with the expense |
| `Cost Category` | High-level cost category |
| `Date` | Expense date |

#### 5️⃣ Table: dim_date

The `dim_date` table is a dedicated date dimension used to support time-based analysis across revenue and expense data.

| Column Name | Description |
|---|---|
| `Date` | Calendar date used to connect financial data with time-based analysis |

#### 6️⃣ Table: dim_Business Line

The `dim_Business Line` table contains the business line master data used to filter and compare financial performance.

| Column Name | Description |
|---|---|
| `Business Line` | Business line name |
| `Business Line ID` | Unique identifier for each business line |

### 🔗 Data Model

<img width="855" height="642" alt="image" src="https://github.com/user-attachments/assets/d7779100-318f-4f75-b21b-ef4794007b57" />
