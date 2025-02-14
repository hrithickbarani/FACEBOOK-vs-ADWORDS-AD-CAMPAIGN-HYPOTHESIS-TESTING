# Advertisement Campaign Analysis: Facebook vs. AdWords

## Project Overview
This project analyzes the performance of two advertising campaigns—Facebook and AdWords—conducted over the year 2019. The goal is to determine which platform is more effective in terms of **conversions**, **clicks**, and **cost-effectiveness**. By identifying the better-performing platform, we aim to optimize advertising strategies and maximize ROI for future campaigns.

---

## Business Problem
As a marketing agency, our primary objective is to maximize the return on investment (ROI) for our clients' advertising campaigns. We conducted two ad campaigns—one on Facebook and the other on AdWords—and need to determine which platform yields better results in terms of **clicks**, **conversions**, and **cost-effectiveness**. By identifying the most effective platform, we can allocate resources more efficiently and optimize advertising strategies.

---

## Research Question
**Which ad platform is more effective in terms of conversions, clicks, and overall cost-effectiveness?**

---

## Dataset
The dataset contains daily performance metrics for Facebook and AdWords campaigns throughout 2019. Key features include:
- **Date**: The date of the campaign data (January 1, 2019, to December 31, 2019).
- **Ad Views**: Number of times the ad was viewed.
- **Ad Clicks**: Number of clicks received on the ad.
- **Ad Conversions**: Number of conversions resulting from the ad.
- **Cost per Ad**: Cost associated with running the ad campaign.
- **Click-Through Rate (CTR)**: Ratio of clicks to views.
- **Conversion Rate**: Ratio of conversions to clicks.
- **Cost per Click (CPC)**: Average cost incurred per click.

---

## Methodology
### 1. **Data Cleaning and Exploratory Data Analysis (EDA)**
   - Converted the `Date` column to datetime format.
   - Renamed columns for consistency and readability.
   - Cleaned and transformed data by removing special characters (`$`, `%`) and converting columns to appropriate data types.
   - Analyzed distributions of key metrics (e.g., ad views, clicks, conversions) for both platforms.

### 2. **Key Insights from EDA**
   - **AdWords** has more **ad views** and **clicks** per day than Facebook.
   - **Facebook** has more **ad conversions** per day than AdWords.
   - **Facebook** has a higher **Click-Through Rate (CTR)** and **Conversion Rate** than AdWords.
   - **Facebook** is more cost-effective, with lower **Cost per Click (CPC)** and **Cost per Ad**.

### 3. **Hypothesis Testing**
   - Conducted a t-test to compare the mean conversions of Facebook and AdWords.
   - **Result**: Facebook has significantly higher conversions than AdWords (p-value < 0.05).

### 4. **Cost-Effectiveness Analysis**
   - Calculated key metrics:
     - **CPC (Cost Per Click)**
     - **CTR (Click-Through Rate)**
     - **CPM (Cost Per Mille)**
     - **CPCV (Cost Per Completed View)**
   - **Findings**:
     - Facebook has lower **CPC** and **CPCV** but higher **CTR** and **CPM** compared to AdWords.
     - Facebook is more cost-efficient and engaging.

### 5. **Regression Analysis**
   - Built a Linear Regression model to predict Facebook conversions based on clicks.
   - **R² Score**: 77.52% (indicating a strong predictive power).
   - **MAE**: 1.32 (minimal error, indicating accurate predictions).

### 6. **Trend Analysis**
   - Analyzed conversions by **weekday** and **month**:
     - **Weekdays**: Highest conversions on **Mondays** and **Tuesdays**.
     - **Months**: Overall upward trend, with dips in **February, April, June, August, and November**.

---

## Key Findings
1. **Facebook outperforms AdWords** in terms of **conversions**, **CTR**, and **cost-effectiveness**.
2. **AdWords** generates more **ad views** and **clicks**, but these do not translate into higher conversions.
3. **Facebook** has a stronger correlation between **clicks** and **conversions** (0.874) compared to AdWords (0.45).
4. **Cost per conversion** is lower on Facebook, making it a more cost-effective platform.
5. **Mondays and Tuesdays** are the best days for conversions on Facebook.
6. **July to December** are the most cost-effective months for Facebook campaigns.

---

## Recommendations
1. **Allocate more resources to Facebook** advertising, as it delivers higher conversions and better ROI.
2. **Optimize AdWords campaigns** by identifying factors that limit conversions despite higher clicks.
3. **Focus on high-conversion periods**:
   - Increase ad spend on **Mondays and Tuesdays**.
   - Capitalize on cost-effective months (**July to December**).
4. **Use the Linear Regression model** to predict conversions based on clicks and set realistic campaign goals.

---

## Tools and Technologies
- **Programming Language**: Python
- **Libraries**: Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, SciPy
- **Visualization**: Matplotlib, Seaborn
- **Statistical Analysis**: Hypothesis Testing, Linear Regression

---
