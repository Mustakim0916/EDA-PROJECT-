Project Overview — Nike Sales Data EDA

This project performs Exploratory Data Analysis (EDA) on the Nike Sales Dataset, which contains detailed information about Nike’s product sales across different regions, sales channels, and categories.

The goal of this project is to:

Understand how Nike’s sales, pricing, and profit behave across different product lines.

Detect patterns, anomalies, and insights that can help optimize sales strategy.

Clean the dataset, handle missing values, and visualize the key trends.

🧾 Dataset Summary

File Name: Nike_Sales_Uncleaned.csv
Total Rows: 2500
Columns: 13

Column	Description
Order_ID	Unique ID for each order
Gender_Category	Target gender (Men, Women, Kids)
Product_Line	Type/category of product (Running, Soccer, Training, etc.)
Product_Name	Product model name
Size	Product size (S, M, L, XL)
Units_Sold	Quantity sold
MRP	Maximum Retail Price
Discount_Applied	Discount percentage
Revenue	Total revenue generated
Order_Date	Date of the order
Sales_Channel	Mode of sale (Online / Retail)
Region	City/region where sale occurred
Profit	Profit earned on that sale
⚙️ Steps Performed in EDA

Data Loading & Inspection

Imported dataset using Pandas.

Checked structure, column types, and null values.

Observed missing data in MRP, Units_Sold, and Discount_Applied.

Data Cleaning

Handled null values using dropna() or fillna() as needed.

Removed duplicate records.

Converted Order_Date to datetime format.

Removed invalid or negative revenue values.

Feature Understanding

Analyzed numeric distributions (MRP, Profit, Revenue).

Studied categorical data like Gender_Category, Product_Line, and Region.

Visualization & Analysis

Histograms for price, revenue, and profit distribution.

Countplots for gender and sales channels.

Scatterplots to explore relationships (e.g., MRP vs Profit).

Trend analysis of revenue over time.

Advanced Exploration

Created new columns such as Profit_Status using list comprehension.

Used iloc, loops, and filtering to extract insights.

Detected records with inconsistent or missing sales info.

📈 Key Insights

Majority of sales came from the Online channel, but Retail sales generated higher profits on average.

Running and Soccer product lines dominate overall sales volume.

Most products fall in the mid-range MRP (₹3000–₹7000).

Some records have revenue = 0 or missing MRP, indicating incomplete transactions or data entry issues.

Profit distribution is positively skewed — a few products contribute heavily to overall profit.

The KDE curves in visualizations helped identify the most common price and profit ranges.

🧰 Technologies Used

Python

Pandas – for data manipulation

NumPy – for numerical operations

Matplotlib / Seaborn – for data visualization

Jupyter Notebook – for analysis and reporting

🪶 Example Visualizations

Distribution of Product Prices (MRP)

Profit Distribution (only positive profits)

Revenue Trend Over Time

Count of Orders by Gender Category

Scatterplot of MRP vs Profit

💡 Learning Outcomes

Gained understanding of retail data cleaning and feature handling.

Learned to perform EDA using Pandas, Seaborn, and Matplotlib.

Practiced writing analytical queries without groupby() using loops, list comprehensions, and iloc.

Strengthened skills in interpreting real-world data and generating business insights.

📝 README.md (For GitHub)

You can copy this below section directly into your GitHub README file 👇

# 👟 Nike Sales Data - Exploratory Data Analysis (EDA)

### 📘 Overview
This project focuses on performing **Exploratory Data Analysis (EDA)** on Nike’s sales data.  
The dataset contains details about product lines, gender categories, regions, profits, and revenues.  
The goal is to clean, explore, and visualize the data to uncover sales trends and actionable insights.

---

### 📂 Dataset Information
**File:** `Nike_Sales_Uncleaned.csv`  
**Rows:** 2500  
**Columns:** 13  

| Column | Description |
|--------|-------------|
| Order_ID | Unique ID for each order |
| Gender_Category | Target gender (Men, Women, Kids) |
| Product_Line | Product type (Running, Soccer, Training, etc.) |
| Product_Name | Nike product model |
| Size | Size of the product |
| Units_Sold | Quantity sold |
| MRP | Product price |
| Discount_Applied | Discount rate applied |
| Revenue | Total revenue generated |
| Order_Date | Date of the order |
| Sales_Channel | Online or Retail |
| Region | Location of sale |
| Profit | Profit from sale |

---

### ⚙️ Steps in the Project
1. **Data Loading & Cleaning** – Checked nulls, removed duplicates, corrected formats  
2. **Exploratory Data Analysis** – Visualized prices, revenue, profits, and regions  
3. **Feature Analysis** – Investigated patterns in gender, category, and sales channels  
4. **Advanced Analysis** – Used `iloc`, loops, and list comprehensions for deeper insights  
5. **Visualization** – Created histograms, scatterplots, and KDE-based distribution plots  

---

### 📊 Key Insights
- Running & Soccer categories generate the highest sales.  
- Online orders are more frequent, but retail stores yield better profits.  
- Most Nike products are priced between ₹3000–₹7000.  
- Some records show missing values in price or units sold, requiring cleaning.  
- Profit distribution is positively skewed, showing few high-profit sales.  

---

### 🧰 Tech Stack
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

### 💡 Learnings
- Data cleaning and wrangling with Pandas  
- Visualization and interpretation with Seaborn & Matplotlib  
- Using loops, list comprehensions, and `iloc` for custom EDA  
- Turning raw data into meaningful business insights  

---

### 📸 Example Visuals
- Distribution of Product Prices  
- Profit Distribution (Positive Only)  
- Revenue Trend Over Time  
- Count of Orders by Gender Category  
- MRP vs Profit Relationship  

---

### 👨‍💻 Author
**MUSTAKIM JAMAL MULLA**  
