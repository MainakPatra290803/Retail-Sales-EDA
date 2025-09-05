# 🛒 Advanced Retail Sales EDA (Superstore Dataset)

## 📌 Project Overview
This project performs **Exploratory Data Analysis (EDA)** on the **Sample Superstore dataset**, a popular dataset for retail analytics.  
The goal is to extract actionable insights, detect patterns, and demonstrate data analysis skills using Python.  
The analysis includes:
- Data cleaning & preprocessing
- Exploratory statistics
- Outlier detection (IQR & boxplots)
- Correlation analysis
- Probability distributions (Normal, Binomial, Poisson)
- Hypothesis testing (Manual ANOVA)
- Business insights with visualizations

This project is designed as a **resume-quality portfolio project** to showcase end-to-end data analysis capability.

---

## 📂 Dataset
- **Name**: `SampleSuperstore.csv`
- **Source**: Kaggle / Tableau sample dataset
- **Rows**: ~10,000 orders
- **Columns**:
  - Categorical: Category, Sub-Category, Region, State, Segment, Ship Mode
  - Numerical: Sales, Profit, Quantity, Discount
  - Dates: Order Date, Ship Date

---

## ⚙️ Tech Stack
- **Language**: Python 3.x  
- **Libraries**:
  - `pandas` → data manipulation
  - `numpy` → numerical calculations
  - `matplotlib`, `seaborn` → visualization
- No external statistical libraries (like `scipy`) were used — all tests (ANOVA, IQR) were coded manually.

---

## 📊 Analysis Workflow
### **0. CONFIG**
- Import libraries, set visualization style, create output directory

### **1. Load Data**
- Read `SampleSuperstore.csv`
- Standardize column names
- Convert date fields and numeric columns

### **2. Data Cleaning**
- Handle duplicates
- Check and handle missing values
- Create derived features:
  - Profit Margin
  - Ship Delay (days)
  - Year, Month, Weekday, Quarter from Order Date

### **3. Descriptive Statistics**
- Dataset overview (shape, datatypes, summary stats)
- Frequency distributions of key columns

### **4. Outlier Detection**
- **IQR Method** for numerical columns
- **Boxplots** for Sales, Profit, Profit Margin, Revenue per Unit
- Mark and count outliers

### **5. Correlation Analysis**
- Heatmap of numerical features (Sales, Profit, Discount, Quantity, Profit Margin)

### **6. Probability Distributions**
- **Normal Distribution**: Sales & Profit histograms with KDE
- **Binomial Distribution**: Probability of Profit vs Loss orders
- **Poisson Distribution**: Orders per day

### **7. Business Insights (Visual EDA)**
- Sales & Profit trends (Yearly, Monthly, Quarterly)
- Region & Category performance
- State-wise Top & Bottom performers
- Sub-Category sales/profit breakdown
- Discount impact on Profit Margin
- Shipping delay analysis

### **8. Hypothesis Testing**
- **Manual ANOVA**: Test if Profit differs significantly across Regions
- Effect size calculated via **eta-squared**

---

## 📌 Key Insights
- High discounts reduce profit margins drastically.  
- Some sub-categories (e.g., Tables, Bookcases) are loss-making despite high sales.  
- The South region shows lower average profit compared to others.  
- Profitability varies strongly across product categories and regions.  
- Shipping delays vary slightly by region but are generally within a few days.  

---

## 📷 Sample Visualizations
- Correlation Heatmap  
- Boxplot of Profit Margin by Category  
- Sales vs Profit Scatterplot  
- Profitability vs Discounts (Binomial Model)  
- Orders per Day Distribution (Poisson Model)  




