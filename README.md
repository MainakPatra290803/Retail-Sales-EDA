# 🛒 Retail Sales EDA (Sample Superstore Dataset)

![Retail Banner](https://i.imgur.com/m63hK6F.png)

---

## 📌 Project Overview  

This project performs a **comprehensive Exploratory Data Analysis (EDA)** on the **Sample Superstore dataset**, a widely used dataset in analytics and data science.  

The goal is **not just visualization**, but also:  
- Identifying **business problems**  
- Applying **statistical methods** (IQR, ANOVA, hypothesis testing)  
- Modeling **uncertainty using probability distributions**  
- Delivering **actionable business insights**  

This project is structured like a **real data science workflow** and is designed to be **resume-quality**.

---

## 🎯 Project Objectives  

We aim to answer critical **business questions**:  

1. Which categories and sub-categories are most profitable?  
2. How do discounts impact profitability?  
3. Which regions and states contribute most to sales and profit?  
4. Do shipping modes affect profitability and customer satisfaction?  
5. Are there seasonal or yearly sales patterns?  
6. Where are the biggest risks of losses (products, locations, discounts)?  
7. Can inferential statistics validate group differences?  
8. How can probability distributions model business events?  

---

## 📂 Project Workflow (Step-by-Step)

### **1️⃣ Import Libraries & Configuration**  
- `pandas` → data manipulation  
- `numpy` → numerical calculations  
- `matplotlib`, `seaborn` → visualization  
- Set seaborn style for better aesthetics  

---

### **2️⃣ Load & Explore Data**  
- Load dataset (`SampleSuperstore.csv`)  
- Normalize column names  
- Check shape, datatypes, head, duplicates, and missing values  

📸 *Example:* Head of dataset  

---

### **3️⃣ Data Cleaning & Feature Engineering**  
- Handle missing values  
- Drop duplicates  
- Convert `order_date` and `ship_date` to datetime  
- Feature engineering:  
  - `year`, `month`, `weekday`, `quarter`  
  - `profit_margin = profit / sales`  
  - `ship_delay_days = ship_date - order_date`  

📸 *Example:* Missing value heatmap  

---

### **4️⃣ Descriptive Statistics**  
- Summary stats (mean, median, mode, std)  
- Understand sales, profit, discount, and quantity distributions  

📸 *Example:* Table of descriptive stats  

---

### **5️⃣ Outlier Detection (IQR + Boxplots)**  
- Compute Q1, Q3, IQR for numeric variables  
- Identify outliers as values outside `[Q1 - 1.5×IQR, Q3 + 1.5×IQR]`  
- Plot boxplots to visualize outliers  

📸 *Example:* Boxplot of Sales by Category  

---

### **6️⃣ Univariate & Bivariate Analysis**  
- Histograms for **Sales** and **Profit** distributions  
- Scatterplot of **Discount vs Profit**  
- Countplots for **Category** and **Region**  

📸 *Example:* Histogram of Sales  

---

### **7️⃣ Correlation Analysis**  
- Correlation heatmap among numeric variables  
- Insights:  
  - Discounts strongly reduce profit  
  - Sales and profit only moderately correlated  

📸 *Example:* Correlation Heatmap  

---

### **8️⃣ Inferential Statistics**  

#### **a. Hypothesis Testing**  
- Hypothesis: Do discounts significantly reduce profits?  
- Compare average profit for orders with vs without discount  

#### **b. ANOVA (Manual)**  
- Test whether mean profit differs significantly across **regions**  
- Compute F-statistic and effect size (η²)  

📸 *Example:* ANOVA summary table  

---

### **9️⃣ Probability Distributions**  

- **Normal Distribution** → Fit Sales & Profit  
- **Binomial Distribution** → Probability of order being profitable  
- **Poisson Distribution** → Model number of orders per day  

📸 *Example:* Sales Histogram with Normal Fit  

---

### **🔟 Business Insights (from Analysis)**  

✔ **Category-Level**  
- Technology → highest profits  
- Furniture → high sales but lower profitability  

✔ **Discount Impact**  
- High discounts often → losses  
- Optimal discount strategy needed  

✔ **Regional Performance**  
- West → highest revenue & profit  
- Central → inconsistent performance  

✔ **Shipping Modes**  
- Same-day shipping → costly, less profitable  
- Standard shipping → most balanced  

✔ **Geographic Risk**  
- Profits concentrated in few states (CA, NY)  
- Expansion opportunities in low-performing regions  

📸 *Example:* State-wise Profit Heatmap  

---

### **1️⃣1️⃣ Extended Business Insights**  

- **Top States by Sales** → CA, NY lead the market  
- **Sub-Categories** → Phones & Chairs drive revenue, but Chairs often unprofitable  
- **Yearly Trends** → Steady sales growth with seasonal peaks  
- **Customer Analysis** → Few high-value customers drive large share of revenue  
- **High Discounts → Losses** → Need pricing optimization  

---

## 📊 Tools & Libraries Used  

- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  








