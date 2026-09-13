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

## 🧠 Design Thinking Process
### 1️⃣ Empathize
<img width="1942" height="809" alt="image" src="https://github.com/user-attachments/assets/227d8e3b-62f1-4c8f-a28e-12da57e9189f" />


<img width="1774" height="887" alt="image" src="https://github.com/user-attachments/assets/b7263a6c-6f0e-4ab2-95cd-daa55a4f8662" />

### 2️⃣ Define point of view


<img width="1780" height="883" alt="image" src="https://github.com/user-attachments/assets/3e61125a-2957-442d-b228-0eb1bb6e1ee2" />

### 3️⃣ Ideate

## 📊 Key Insights & Visualizations

### 🔍 Dashboard Preview

### 📋 Overview

<img width="1346" height="756" alt="image" src="https://github.com/user-attachments/assets/694d3d29-ae0e-4666-94bb-a3847ad33716" />



* Revenue peaked around the middle of the year but showed a slight overall downward trend.
* Sports Equipment generated the highest revenue but had a lower net profit margin than Sportswear, while Nutrition & Food Supplements was loss-making.
* Overall, the business maintained a relatively healthy growth quality, with profit margins improving alongside revenue.

### 📋 Business Line Performance


<img width="1533" height="856" alt="image" src="https://github.com/user-attachments/assets/03a24e5b-362d-4fdf-a9b8-225620f855a7" />

* Sportswear had the highest gross margin at 70%, followed by Sports Equipment at 59% and Nutrition & Food Supplements at 45%.
Nutrition & Food Supplements had an unusually high growth-cost ratio, mainly driven by R&D expenses, putting significant pressure on profitability and resulting in a net loss.
* Monthly performance varied across business lines, highlighting differences in revenue generation and profitability over time.
* Sports Equipment consistently generated the highest revenue but had a significantly lower net profit margin than Sportswear (26% vs. 40%), making profitability more sensitive to Sales and Marketing costs.
* Sportswear generated less revenue than Sports Equipment but still made a significant contribution to total revenue. Its high margin and relatively low Sales costs indicate strong potential for scaling, while profitability remains sensitive to Marketing costs.
  
### 📋 Cost Structure

<img width="1526" height="859" alt="image" src="https://github.com/user-attachments/assets/abc6baa3-7f57-4abd-8527-789b26b83e8f" />

* The Fixed Cost / Revenue ratio showed an upward trend, indicating that fixed costs were growing faster than revenue.
* This increasing fixed-cost burden may be limiting profitability and should be monitored to ensure that cost growth is supported by sufficient revenue generation.

## Key Insights & Recommendations

| Perspective | Insight | Recommendation |
|---|---|---|
| **Overview** | • Revenue peaks mid-year but shows a slight downward trend afterward.<br>• Profit margin increases with revenue, indicating relatively healthy growth quality.<br>• Sports Equipment leads revenue but has lower profitability, while Nutrition is loss-making. | • Prioritize growth based on **profitability and scalability**, not revenue alone. |
| **Business Line** | • **Sportswear:** Highest gross margin (70%) and net margin (40%), with strong scalability potential.<br>• **Sports Equipment:** Highest revenue but lower net margin (26%) and higher sensitivity to sales & marketing costs.<br>• **Nutrition:** Low gross margin (45%) and high R&D cost growth, resulting in losses. | • Increase **marketing investment in Sportswear** to leverage its high margin and scalability.<br>• Optimize **Sales & Marketing spending** for Sports Equipment and monitor ROI.<br>• Reassess **R&D efficiency** in Nutrition. |
| **Cost Structure** | • Fixed cost / revenue is increasing.<br>• New capacity investments mainly support Sports Equipment but have not yet generated proportional revenue. | • Improve **capacity utilization** and revenue generation before further expanding fixed costs.<br>• Review the **ROI of existing investments**. |

