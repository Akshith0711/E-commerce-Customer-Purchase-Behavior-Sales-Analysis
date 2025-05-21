# 🛒 E-commerce Customer Purchase Behavior & Sales Analysis

This is a data analysis project using customer transactions from an online retail store. I used Python and Jupyter Notebook to clean the data and explore patterns in customer purchases.

## 📁 Dataset Information

- **Name**: Online Retail II (2009–2010)
- **Source**: UCI Machine Learning Repository
- **File used**: `Year 2009-2010.csv`

---

##  What I Did So Far

### Day 1: Data Cleaning

- Opened the dataset in Jupyter Notebook.
- Removed rows with missing customer information.
- Removed canceled orders (invoices starting with 'C').
- Removed rows with negative or zero quantity or price.
- Created a new column called `TotalPrice` (Quantity × Price).
- Converted the invoice date to datetime format.
- Saved the cleaned file as: `cleaned_online_retail.csv`

### Day 2: Data Analysis

I explored the data to find interesting patterns:

- Total number of transactions
- Number of unique products
- Countries with most sales
- Top 10 customers by how much they spent
- Top 10 products by quantity sold
- Monthly trend of total sales

I also created a **line chart** to see how sales changed over each month.

---

##  Tools I Used

- Python (pandas, matplotlib)
- Jupyter Notebook

---

##  How to Run

1. Download the dataset (`Year 2009-2010.csv`) from UCI.
2. Run the notebook in Jupyter.
3. Start with the Day 1 code to clean the data.
4. Then use the cleaned data for Day 2 analysis.

---
Day 3: RFM Analysis - Customer Segmentation
 ## 📌 What I Did on Day 3

###  RFM Analysis

- **Recency**: How recently a customer made a purchase.
- **Frequency**: How often a customer made a purchase.
- **Monetary**: How much money the customer spent.

###  Steps Taken

1. Loaded the cleaned dataset.
2. Converted `InvoiceDate` to datetime format.
3. Set a **reference date** for Recency calculation.
4. Grouped by `CustomerID` to calculate:
   - Recency: Days since last purchase
   - Frequency: Number of invoices
   - Monetary: Total amount spent
5. Scored each metric into 1–5 scale.
6. Created `RFM_Segment` and `RFM_Score` for customer grouping.

---

##  Insights

- Customers with high **RFM scores (e.g. 555)** are the most loyal and valuable.
- Low scores (e.g. 111) indicate inactive or low-value customers.
- This segmentation is helpful for targeting marketing strategies like:
  - VIP rewards
  - Re-engagement campaigns
  - Upselling opportunities

---

##  What I Learned

- How to compute Recency, Frequency, and Monetary metrics.
- The power of RFM in understanding customer behavior.
- How to score and segment customers using pandas.
- Improved data grouping and lambda function usage.

---

##  Sample Output

| CustomerID | Recency | Frequency | Monetary | R_Score | F_Score | M_Score | RFM_Segment | RFM_Score |
|------------|---------|-----------|----------|---------|---------|---------|-------------|-----------|
| 12345.0    |   12    |     4     | 500.00   |    4    |    3    |    2    |     432     |     9     |

---
##  Tools Used

- Python
- pandas
- Jupyter Notebook
  Day 4 Goal:
   Analyzed how many customers return in future months after their first purchase and visualize it using a cohort heatmap.

 What is a Cohort?
  A cohort is a group of customers who made their first purchase in the same month.

  We track these groups to see:

   How long they stay active

   When they return

   How loyal they are over time

✅Key Steps:
1.  Data Preparation:
Cleaned and formatted the dataset from previous days.

Converted invoice dates to datetime format.

Removed missing or canceled transactions.

2.  Created Cohorts:
Extracted:

CohortMonth: when a user made their first purchase.

InvoiceMonth: when a user made any purchase.

Calculated CohortIndex → how many months later a customer came back.

3.  Created Cohort Tables:
Cohort Table: Shows how many users returned each month.

Retention Table: Shows the percentage of returning users.

4.  Visualized Retention with a Heatmap:
Used seaborn to create a retention heatmap.

Darker colors = more users returned that month.

Easy to spot which cohorts are most loyal.

 Example Insights:
Some customer groups came back regularly for 4–6 months.

Others stopped purchasing after their first visit.

Helps marketing teams know which months brought high-retention customers.

 Tools Used:
pandas for data manipulation

matplotlib & seaborn for visualization

datetime for date handling

##  About Me

I'm learning data science and building real-world projects to grow my skills. This is one of my practice projects.

