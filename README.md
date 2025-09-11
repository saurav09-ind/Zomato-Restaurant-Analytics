# 🍴 Zomato Restaurant Analytics

An end-to-end **data science and statistical modeling project** on the Zomato restaurant dataset.  
The goal of this project is to explore restaurant-related data, perform **EDA (Exploratory Data Analysis)**, and apply **statistical hypothesis testing** to gain actionable insights.  

---

## 🔍 Project Overview
Zomato is a popular restaurant discovery and food delivery platform. This project analyzes restaurant-level data to uncover patterns in ratings, online ordering, cost, and location.  

Key objectives:
- Perform **data cleaning & preprocessing**.  
- Conduct **exploratory data analysis** for insights.  
- Apply **statistical hypothesis tests** (t-test, chi-square, ANOVA, correlation).  
- Interpret results to understand customer and restaurant behavior.  

---

## 🗂 Dataset
The dataset contains restaurant attributes from Zomato.  

**Key Columns:**
- `rate` – Restaurant rating  
- `votes` – Number of customer votes  
- `approx_cost(for two people)` – Average cost for two  
- `online_order` – Online order availability (Yes/No)  
- `book_table` – Table booking availability (Yes/No)  
- `location` – Restaurant location  
- `cuisines` – Cuisine types offered  

---

## ⚙️ Project Workflow

### 1. Data Preprocessing
- Removed duplicates and irrelevant columns (`url`, `address`, `menu_item`, etc.).  
- Handled missing values.  
- Converted cost values into numeric.  
- Cleaned ratings column for analysis.  

### 2. Exploratory Data Analysis (EDA)
- Distribution of restaurant ratings and votes.  
- Analysis of costs vs ratings.  
- Online ordering and booking availability.  
- Location-wise restaurant density and performance.  

### 3. Statistical Modeling & Hypothesis Testing

Performed several statistical tests to validate assumptions:  

#### 📌 Hypothesis 1: Online Order vs Ratings
- **Test:** Independent t-test  
- **Result:**  
  - T-Statistic: `13.8161`  
  - P-Value: `2.49e-43`  
  - ✅ *Significant difference found*: Restaurants with **online ordering** have higher ratings.  

---

#### 📌 Hypothesis 2: Table Booking vs Online Order
- **Test:** Chi-Square Test  
- **Result:**  
  - Chi2: `0.1930`  
  - P-Value: `0.6603`  
  - ❌ *No significant relationship*: Table booking and online ordering are independent.  

---

#### 📌 Hypothesis 3: Location vs Ratings
- **Test:** One-Way ANOVA  
- **Result:**  
  - F-Statistic: `533.58`  
  - P-Value: `0.0`  
  - ✅ *Significant difference*: Restaurant ratings vary significantly across locations.  

---

#### 📌 Hypothesis 4: Cost vs Rating
- **Test:** Pearson Correlation  
- **Result:** Weak correlation observed between cost and ratings (not statistically significant in this dataset).  

---

## 📈 Key Insights
- Online ordering is positively associated with higher restaurant ratings.  
- Table booking availability does not influence online order adoption.  
- Location plays a crucial role in determining restaurant ratings.  
- Price is not a strong indicator of restaurant quality.  

---

## 🛠️ Tech Stack
- **Python**: Pandas, NumPy, Scipy, Scikit-learn  
- **Visualization**: Matplotlib, Seaborn  
- **Statistics**: T-tests, Chi-Square, ANOVA, Correlation  
- **Notebook**: Jupyter  

---

