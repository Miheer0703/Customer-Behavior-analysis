# 🛍️ Customer Shopping Behavior Analysis

End-to-end data analytics project analysing **3,900 retail purchases** to uncover spending patterns, customer segments, product preferences and subscription behaviour. The data was cleaned in **Python**, analysed in **MySQL** and visualised in **Power BI**, ending with data-driven business recommendations.


---

## 🛠️ Tools & Technologies

| Stage | Tools |
|---|---|
| Data cleaning & feature engineering | Python (pandas, NumPy) |
| Business analysis | MySQL |
| Dashboard | Power BI |
| Reporting | PDF report, PowerPoint presentation |

---

## 📁 Dataset

- **3,900 rows × 18 columns**, one purchase per customer
- **Demographics:** age, gender, location, subscription status
- **Purchase details:** item, category, purchase amount, season, size, colour
- **Behaviour:** discount applied, promo code used, previous purchases, purchase frequency, review rating, shipping type
- **Missing data:** 37 values in Review Rating

---

## 🔄 Project Workflow

### 1️⃣ Data Cleaning in Python
- Explored the data with `df.info()` and `df.describe()`
- Filled 37 missing review ratings with each category's **median rating**
- Renamed columns to **snake_case**
- Added new features: `age_group` (binned ages) and `purchase_frequency_days`
- Dropped `promo_code_used`, which duplicated `discount_applied`
- Loaded the cleaned data into **PostgreSQL**

### 2️⃣ Business Analysis in SQL
Answered 10 business questions:
1. Revenue by gender
2. Customers who used discounts but still spent above average
3. Top 5 products by average rating
4. Average purchase: Standard vs Express shipping
5. Subscribers vs non-subscribers: spend and revenue
6. Five products most often bought on discount
7. Customer segments: New, Returning and Loyal
8. Top 3 products in each category
9. Do repeat buyers (more than 5 purchases) subscribe more?
10. Revenue by age group

### 3️⃣ Dashboard in Power BI
- **KPI cards:** number of customers, average purchase amount, average review rating
- **Filters:** subscription status, gender, category, shipping type
- **Charts:** subscription share, revenue and orders by category, revenue and orders by age group

---

## 📊 Key Insights

| Metric | Result |
|---|---|
| 💰 Total revenue | **$233,081** |
| 🛒 Average purchase | **$59.76** |
| ⭐ Average review rating | **3.75 / 5** |
| 👨 Revenue from male customers | $157,890 (68%) |
| 👩 Revenue from female customers | $75,191 (32%) |
| 🔁 Loyal customers | 3,116 (80%) |
| 📩 Subscribers | 1,053 (27%) |
| 🏷️ Purchases with a discount | 1,677 (43%) |
| 🏆 Top-rated product | Gloves (3.86) |
| 🚚 Average order, Express vs Standard | $60.48 vs $58.46 |
| 🎯 Highest-revenue age group | Young Adult ($62,143) |

**What this means:**
- **Subscriptions don't change behaviour:** subscribers spend $59.49 per order vs $59.87 for non-subscribers.
- **Repeat buyers don't subscribe more:** only 27.6% of them subscribe, the same as the overall rate.
- **Discounts are heavily used:** Hats, Sneakers and Coats are bought on discount about half the time.
- **Clothing and Accessories** bring in about three-quarters of total revenue.
- **Revenue is spread evenly** across age groups: only $6.4K separates the highest and lowest.

---

## 💡 Business Recommendations

1. **Boost subscriptions:** offer exclusive benefits that give customers a reason to subscribe.
2. **Reward loyalty:** use a loyalty programme to move the 701 returning customers into the Loyal segment.
3. **Review the discount policy:** reduce discounts on heavily discounted products to protect margin.
4. **Position top products:** feature top-rated and best-selling items, such as Sandals, Jewelry and Blouses, in campaigns.
5. **Target marketing:** focus on high-revenue age groups and customers who choose express shipping.

---

## 📂 Repository Structure

```
customer-shopping-behavior-analysis/
├── dashboard/      Power BI dashboard (.pbix)
├── sql/            Mysql  queries (.sql)
├── notebooks/      Python data cleaning notebook (.ipynb)
├── README.md
├── csv /           Customer Shopping Behavior.csv
```

## 👤 Author

**Miheer**
- GitHub: [Miheer0703](https://github.com/Miheer0703)
- LinkedIn: [www.linkedin.com/in/miheer-sawant]

⭐ *If you found this project useful, consider giving it a star!*
