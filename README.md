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

##  What's Next

I will:
- Continue to Day 3 with customer segmentation.
- Later build a dashboard using Power BI.

---

##  About Me

I'm learning data science and building real-world projects to grow my skills. This is one of my practice projects.

