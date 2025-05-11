# 📊 A/B Testing for Marketing Campaign Efficiency

## 📝 Background

As part of a marketing agency’s strategic initiatives, this project aims to identify the more effective advertising platform between **Facebook** and **Google AdWords**. The ultimate goal is to **maximize ROI** by analyzing daily ad campaign data to determine which platform delivers better performance in terms of **clicks, conversions, and cost-efficiency**.

Understanding platform performance helps in making **data-driven decisions** about resource allocation and optimizing advertising strategies for better client outcomes.

---

## ❓ Business Problem
As a marketing agency, our primary objective is to maximize ROI for our clients’ advertising campaigns. We conducted two campaigns on Facebook and AdWords, and we aim to identify the more effective platform. This will help us allocate advertising budgets more strategically and optimize future campaigns for higher returns.

---

## 🎯 Objective

To determine which advertising platform—**Facebook** or **AdWords**—provides:

* Higher **conversion rates**
* Better **click-through rates (CTR)**
* Greater **cost-effectiveness** (CPC and CPA)

---

## 📊 Dataset Overview

This analysis is based on 365 daily entries from the year **2019**, capturing essential marketing KPIs from both platforms.

### Features:

* **📅 Date**: Daily record from Jan 1 to Dec 31, 2019
* **👀 Ad Views**: Total impressions per platform
* **🖱 Ad Clicks**: Number of user interactions
* **🔄 Ad Conversions**: Successful conversion events
* **💸 Cost**: Daily ad spend
* **🔗 CTR** *(Click-Through Rate)*: `Clicks / Views`
* **📈 Conversion Rate**: `Conversions / Clicks`
* **💵 CPC** *(Cost per Click)*: `Cost / Clicks`
* **💰 CPA** *(Cost per Acquisition)*: `Cost / Conversions`

---

## 🔍 Methodology

### ✅ Data Cleaning

* Converted date format
* Handled missing values and ensured data integrity

### 📊 Exploratory Data Analysis (EDA)

* Visualized distributions for **CTR**, **Conversion Rate**, **CPC**, and **CPA**
* Identified platform-wise performance trends
* Click and Conversion Distributions: Visualized histograms for Facebook and AdWords.
* Categorized Conversions: Grouped days based on conversion volume to compare platforms.
* Click vs. Conversion Correlation:
* Facebook: Strong correlation (r = 0.87)
* AdWords: Moderate correlation (r = 0.45)



### 📐 Statistical Testing

* **T-tests** to compare metrics (Conversion Rate, CTR, CPC, CPA) between platforms
* **Significance testing** to ensure results aren't due to random variation

### 📊 Hypothesis Testing
* **Null Hypothesis (H₀)**: Facebook conversions ≤ AdWords conversions
* **Alternate Hypothesis (H₁)**: Facebook conversions > AdWords conversions

* **Result**:
   * Facebook Avg Conversions: 11.74
   * AdWords Avg Conversions: 5.98
   * p-value: 9.35e-134 → Null hypothesis rejected



### 🔗 Correlation & Cointegration

* Correlation analysis between clicks and conversions
* Cointegration tests (optional insight) to explore long-run trends between cost and conversions

### 📈 Predictive Modeling

* **Linear regression** model to predict conversions based on clicks
* Evaluated with **R²** and **MSE**

### 📉 Regression Analysis
* **Model**: Linear Regression to predict Facebook conversions based on clicks
* **Performance**: R² = 76.2%
* **Insight**: Higher Facebook ad clicks significantly predict higher conversions

---

## 📈 Key Findings

* **Platform Efficiency**: Facebook outperformed AdWords with **higher conversion rates** and **lower CPC**
* **Ad Spend Strategy**: Recommendation to **shift more budget to Facebook** for better ROI
* **Seasonal Insights**: Time-based patterns suggest certain months perform better—useful for future budget timing

## ✅ Recommendations
* Facebook outperformed AdWords in terms of conversions and conversion consistency.
* Strong evidence suggests reallocating more budget toward Facebook Ads for better ROI.
* Consider experimenting with Facebook ad creatives and targeting to further enhance performance.

---

## 💻 Technologies Used

| Tool                         | Purpose                         |
| ---------------------------- | ------------------------------- |
| **Python**                   | Data analysis and modeling      |
| **Pandas** & **NumPy**       | Data manipulation               |
| **Matplotlib** & **Seaborn** | Data visualization              |
| **SciPy**                    | Hypothesis testing & statistics |
| **Scikit-learn**             | Regression and evaluation       |

---


## ✅ Conclusion

This A/B testing project demonstrates the power of **data-driven marketing**. By systematically comparing ad performance, we delivered actionable insights to optimize future campaigns. Facebook proved to be the stronger platform across key metrics, enabling smarter ad budget decisions.
