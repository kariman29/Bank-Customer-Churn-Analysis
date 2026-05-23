# Bank-Customer-Churn-Analysis
End-to-end EDA project on 10K+ bank customers uncovering churn drivers across demographics, financial profile, and engagement behavior, with actionable retention recommendations.

# 🏦 Bank Customer Churn Analysis — Exploratory Data Analysis (EDA)

An end-to-end **Exploratory Data Analysis** project investigating customer attrition behavior in a retail banking portfolio. The project identifies the **key drivers of churn** across demographics, financial profile, and engagement behavior — and translates the findings into clear, actionable retention strategies presented in an executive briefing.

---

## 🎯 Project Overview

Customer attrition is one of the most costly problems in retail banking — acquiring a new customer can cost 5–7x more than retaining an existing one. This project analyzes **10,127 bank customers** to:

- Quantify the overall churn rate and customer attrition profile
- Identify which **demographic, financial, and behavioral factors** correlate with churn
- Surface **early warning signals** of disengagement
- Recommend **targeted retention strategies** for the highest-risk segments

The analysis is delivered through a clean Jupyter notebook (technical audience) and an **executive briefing presentation** (business audience).

---

## 🛠️ Tools & Technologies

- **Python 3** — Core analysis
- **Pandas / NumPy** — Data manipulation and feature engineering
- **Plotly Express & Graph Objects** — Interactive visualizations
- **Matplotlib / Seaborn** — Supporting statistical plots
- **Jupyter Notebook** — Reproducible analysis workflow
- **PowerPoint** — Executive-level reporting

---

## 📊 Dataset

- **Source:** Bank Churners dataset (Kaggle)
- **Records:** 10,127 customers
- **Features:** 20+ attributes covering demographics, account info, card details, and 12-month transaction behavior
- **Target Variable:** `Attrition_Flag` (Existing Customer / Attrited Customer)

### Data Cleaning Steps
- Removed irrelevant columns (`CLIENTNUM`, pre-built Naive Bayes classifier columns)
- Converted `Credit_Limit` and `Avg_Open_To_Buy` to integer types
- Verified no missing values across the dataset
- Created derived feature groups (Age Groups, Credit Limit Groups, Transaction Amount Groups) for segmentation

---

## 🔍 Key Insights & Findings

### 1. Overall Churn Rate
- **16.1%** of customers have churned — a meaningful retention gap worth addressing.

### 2. Demographics
| Factor | Insight |
|--------|---------|
| **Age** | Churn rate climbs to ~20% in the **65+** segment, suggesting retention issues among older customers |
| **Marital Status** | **Single** and **Unknown** marital status segments show the highest churn (~17%) |
| **Income** | Highest churn observed in **$120K+** earners (~17.3%) — premium segment is at risk |

### 3. Financial Profile
| Factor | Insight |
|--------|---------|
| **Credit Limit** | **Very Low** credit limit group has the highest churn (~22.6%) — likely indicating low engagement |
| **Card Category** | **Platinum** cardholders churn at **~25%** — the highest of any tier, suggesting unmet premium expectations |

### 4. Engagement Behavior (Strongest Predictors)
| Factor | Insight |
|--------|---------|
| **Transaction Count** | Customers with **0–20 transactions/year** churn at **~68%** — by far the strongest signal |
| **Transaction Amount** | The **Medium** transaction amount group shows ~37% churn |
| **Banking Relationships** | Customers with only **1–2 products** churn at ~26–28%; those with **6 products** churn at just ~10% |
| **Inactive Months** | Churn risk rises sharply after **3+ months of inactivity** |

---

## 💡 Business Recommendations

1. **Re-engage low-transaction customers (highest priority)** — Customers with fewer than 20 transactions per year represent the largest churn risk. Trigger automated re-engagement campaigns when transaction volume drops.

2. **Build inactivity-based early warning alerts** — Flag customers crossing the **3-month inactivity threshold** for proactive outreach by relationship managers.

3. **Cross-sell to single-product customers** — Customers with only 1–2 banking products are 2.6x more likely to churn than those with 6. Prioritize cross-sell campaigns to deepen relationships.

4. **Audit the Platinum cardholder experience** — A 25% churn rate among premium cardholders signals unmet expectations. Review benefits, service quality, and engagement strategy for this segment.

5. **Target high-income retention** — The $120K+ income segment shows surprisingly high churn. Investigate competitive pressure and tailor premium retention offers.

---

## 📁 Repository Contents

```
📦 Bank-Customer-Churn-Analysis
 ┣ 📄 BankChurnersPROJECT.ipynb                    # Full EDA notebook
 ┣ 📄 BankChurnersPROJECT_report.pdf               # Notebook exported as PDF report
 ┣ 📄 Customer_Attrition_Executive_Briefing.pptx   # Executive-level presentation
 ┗ 📄 README.md
```

---

## 🚀 How to Use

### Option 1 — View the Report
- Open **`BankChurnersPROJECT_report.pdf`** for the full visual report.
- Open **`Customer_Attrition_Executive_Briefing.pptx`** for the business-facing summary.

### Option 2 — Run the Notebook
1. Clone this repository:
   ```bash
   git clone https://github.com/<your-username>/<repo-name>.git
   ```
2. Install required libraries:
   ```bash
   pip install pandas numpy matplotlib seaborn plotly jupyter
   ```
3. Download the **Bank Churners** dataset from Kaggle and update the file path in the notebook.
4. Launch the notebook:
   ```bash
   jupyter notebook BankChurnersPROJECT.ipynb
   ```

---

## 📈 Skills Demonstrated

- **Exploratory Data Analysis (EDA)** with structured, hypothesis-driven investigation
- **Data Cleaning & Feature Engineering** — binning continuous variables into meaningful business segments
- **Statistical Segmentation** — comparing churn rates across categorical and numerical groups
- **Interactive Visualization** with Plotly
- **Business Storytelling** — translating raw findings into actionable recommendations
- **Executive Communication** — packaging technical insights into a stakeholder-ready presentation

---

## 📬 Contact

If you have questions, feedback, or want to connect:

- **GitHub:** [github](https://github.com/kariman29)
- **LinkedIn:** [linkedin-profile](https://www.linkedin.com/in/karimanibrahem45/)

---
