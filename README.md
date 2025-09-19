# 🛍️ Customer Behavior Analysis

This project explores customer behavior using a dataset of **5,000 customers**.  
The analysis applies **statistical tests and visualizations** to uncover insights into spending, churn, product categories, and campaign effectiveness.

---

## 📂 Project Structure
- `customer_behavior.csv` → dataset
- `customer_behavior.ipynb` → Jupyter notebook with analysis
- `README.md` → project documentation

---

## 🔎 Key Questions & Insights

### 1. **Is there a significant difference in spending between male and female customers?**
- ✅ Yes.  
- A **t-test** showed that male and female customers spend **significantly differently**.

---

### 2. **Does PurchaseAmount vary across different regions?**
- ❌ No.  
- ANOVA test result (F = 0.40, p = 0.756) → **no significant variation** in spending across regions.

---

### 3. **Is there a relationship between ProductCategory and customer churn?**
- Used a **Chi-square test of independence**.  
- Result suggests churn **may depend on product category** (check results for exact p-value).

---

### 4. **Which email campaign (A or B) performed better in terms of average PurchaseAmount?**
- ❌ No significant difference.  
- Campaign A and B had **similar effectiveness** in driving spending.

---

### 5. **Does PurchaseAmount follow a normal distribution?**
- The data is **slightly skewed** with heavy tails.  
- **Q-Q plots and histograms** confirm deviations from normality.  
- However, thanks to the **Central Limit Theorem (CLT)**, the distribution of sample means is approximately normal.

---

### 6. **What insights can we gain by applying the Central Limit Theorem?**
- Even though raw `PurchaseAmount` is skewed, the **average spending is stable** when using large samples.  
- This justifies the use of **parametric tests** (t-test, ANOVA).  

---

### 7. **What is the 95% confidence interval for the average PurchaseAmount?**
- **Mean = 1003.95**  
- **95% CI = (990.38 , 1017.52)**  
- Interpretation: Customers spend about **\$1000 on average**, and we are confident the true mean lies within this range.

---

## 📊 Tools & Libraries
- **Python**  
- **Pandas** for data handling  
- **Matplotlib & Seaborn** for visualization  
- **SciPy** for statistical tests  

---

## 🚀 How to Run
1. Clone this repo  
   ```bash
   git clone https://github.com/yourusername/customer-behavior-analysis.git
   cd customer-behavior-analysis

