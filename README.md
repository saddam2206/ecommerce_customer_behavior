
# 🛍️ E-Commerce Customer Behavior Analysis

Welcome to the E-commerce Customer Behavior Analysis project!  
This repository contains a comprehensive data analysis pipeline applied to a dataset of online customers. The goal is to uncover actionable insights from user demographics, purchasing patterns, satisfaction scores, and behavioral data.

---

## 📊 Project Overview

This project is designed around a 3-tiered structure of **insight levels**—ranging from basic to advanced analysis. Each level addresses specific business and analytical questions to help stakeholders understand customer behavior, loyalty, and performance drivers.

The work includes:

- **Exploratory Data Analysis (EDA)**
- **Descriptive & Inferential Statistics**
- **Correlation and Distribution Analysis**
- **Visual storytelling with Matplotlib & Seaborn**

---

## 🧾 Dataset Description

The dataset contains anonymized e-commerce customer records, including:

| Column                  | Description |
|------------------------|-------------|
| Customer ID            | Unique customer identifier |
| Age                    | Customer's age |
| Gender                 | Male, Female, Other |
| Location               | Customer's city/region |
| Product Category       | Type of product purchased |
| Purchase Amount ($)    | Total spent in USD |
| Time Spent on Website  | Minutes per session |
| Device Type            | Device used (Mobile, Desktop, Tablet) |
| Payment Method         | Cash, Card, Bank Transfer, etc. |
| Discount Availed       | Discount used (True/False) |
| Number of Items Purchased | Number of items bought |
| Return Customer        | Whether they are a returning customer |
| Review Score (1–5)     | Product/service rating |
| Delivery Time (days)   | Delivery duration |
| Subscription Status    | Free, Trial, Premium |
| Customer Satisfaction  | Low, Medium, High |

---

## 📌 Questions & Analysis Framework

### 🔹 Level 1: Basic Insights

| Question | Key Outputs |
|----------|-------------|
| Q1. Mean, Median, Mode of Age | Descriptive stats using `.mean()`, `.median()`, `.mode()` |
| Q2. Variance, Std Dev, Z-score (Purchase Amount) | z-score computed with `scipy.stats.zscore` |
| Q3. Top 3 Product Categories | Based on total purchase value (Pie chart included) |
| Q4. Count of Return Customers | Simple `.sum()` on boolean column |
| Q5. Average Review Score | Overall customer feedback (1–5 scale) |
| Q6. Delivery Time by Subscription Type | Bar chart comparing Free vs Premium |
| Q7. How many are subscribed? | Filtered count for Premium |
| Q8. Device Type Usage % | Pie chart and bar chart comparisons |
| Q9. Avg Purchase: With vs Without Discount | Grouped bar comparison |
| Q10. Most Common Payment Method | Pie chart + Mode |

---

### 🔹 Level 2: Intermediate Insights

| Question | Key Outputs |
|----------|-------------|
| Q1. Avg Review Score of Most Used Payment Method | Filtered mean score |
| Q2. Correlation: Time Spent vs Purchase Amount | Weak correlation ⇒ no direct relation |
| Q3. % of Satisfied + Return Customers | Combined condition with `.isin()` and boolean logic |
| Q4. Items Purchased vs Satisfaction | Categorical mapping → heatmap + correlation |
| Q5. 2nd Highest Location by Avg Purchase | `groupby().mean().sort_values()` used |

---

### 🔹 Level 3: Critical Thinking Insights

| Question | Description |
|---------|-------------|
| **Q1. What factors influence returning customers?** | Analyzed both **categorical** and **numerical** variables across Return status with plots & insights |
| **Q2. How do Payment Methods affect Satisfaction and Return Rates?** | Label encoding + heatmap correlation (all near zero ⇒ no significant influence) |
| **Q3. How does Location influence Purchase & Delivery?** | Dual-axis bar chart + insight-rich breakdown |
| **Q4. Summary of Key Insights** | See below ⬇️ |

---

## 🧠 Key Insights Summary

🔹 **Top Influencing Factors for Return Customers:**
- Customers **who received discounts** returned more often
- **Highly satisfied** customers (Review Score 4/5 or High Satisfaction) were likelier to return
- **Premium subscribers** showed slightly higher return rates

🔹 **Location-based Differences:**
- **Khulna** and **Barisal** had the **highest average purchase amounts**
- **Delivery was fastest in Dhaka**, likely due to better logistics infrastructure
- **Rangpur** and **Sylhet** lagged in both delivery time and spending

🔹 **Device Usage:**
- Majority used **Mobile** and **Desktop**, with slight increase in returns from **Tablet users**

🔹 **Payment Method:**
- Most common: **Credit Card**
- However, payment method **did not strongly influence** satisfaction or return behavior

---

## 📈 Visualizations & Techniques

- **Bar charts** for category comparisons
<img width="1783" height="1983" alt="Image" src="https://github.com/user-attachments/assets/d2c67b38-d14c-4bc7-89fb-103f4434ca5d" /> 

- **Pie charts** for proportions
 <img width="465" height="360" alt="Image" src="https://github.com/user-attachments/assets/101ad312-a5eb-42d8-82cb-9ecae156547c" />
- **Correlation heatmaps** to assess relationships
  <img width="639" height="384" alt="Image" src="https://github.com/user-attachments/assets/ef61bac0-45ae-4a92-87eb-735fade8d299" />
- **Count plots & histograms** segmented by return customer status
- **Dual-axis bar charts**  for geographic analysis
 <img width="1184" height="584" alt="Image" src="https://github.com/user-attachments/assets/cedac8da-1bde-42ff-afca-29ef9caaf6df" />

---

## 🛠️ Tools Used

- Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn)
- Jupyter Notebook / Google Colab
- GitHub for version control & documentation

---

## 📂 Repository Structure

```

ecommerce-customer-analysis/
│
├── data/
│   └── ecommerce\_customer\_behavior\_dataset.csv
│
├── notebooks/
│   └── analysis.ipynb
│
├── visuals/
│   └── (Generated plots and charts)
│
├── README.md
└── requirements.txt

```

---

## 📌 Final Note

This project demonstrates how structured data analysis can help businesses:

- Understand customer behavior
- Improve retention strategy
- Optimize logistics by region
- Tailor discount and subscription offerings

Feel free to fork or clone this repo and explore further.  
📬 *For any questions or suggestions, please open an issue or connect with me on LinkedIn.*

---

## 🔗 Connect with Me

**Saddam Hossain**  
📇 [LinkedIn Profile](https://www.linkedin.com/in/saddam-hossain-27a07933a)

---

**⭐️ If you find this project useful, don’t forget to star it!**
