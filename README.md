# Car Insurance Risk Analysis Dashboard

## Project Overview

This project presents a comprehensive analysis of car insurance customer data using Tableau. The objective is to identify key risk factors influencing insurance claims and provide actionable business recommendations for improving underwriting, pricing strategies, and risk management.

The analysis explores customer behavior across geographic, occupational, vehicle, demographic, and behavioral dimensions to uncover patterns associated with higher claim frequency and claim severity.

---

## Objectives

* Identify high-risk customer segments.
* Analyze factors contributing to insurance claims.
* Understand the impact of geography, occupation, vehicle type, and demographics on insurance risk.
* Provide data-driven recommendations for insurance companies.
* Build interactive dashboards to support business decision-making.

---

## Tools & Technologies

* Tableau
* Microsoft Excel
* Data Cleaning & Transformation
* Calculated Fields
* Data Visualization
* Business Intelligence & Analytics

---

## Dashboard Overview

### 1. Geographic Risk Analysis

Focuses on understanding how location influences insurance claims and customer risk.

**Key Metrics:**

* Average Claim Amount
* Average Claim Frequency
* Average Previous Claims
* Customer Distribution by Urbanicity

**Key Finding:**
Urban customers exhibit higher claim amounts and stronger claim histories compared to rural customers.

---

### 2. Occupational Risk Analysis

Analyzes claim behavior across different occupations.

**Key Metrics:**

* Average Claim Amount by Occupation
* Claim Frequency by Occupation
* Risk Score by Occupation
* High-Risk Customer Percentage

**Key Finding:**
Blue-collar customers represent the highest-risk occupational segment.

---

### 3. Vehicle Risk Analysis

Evaluates risk associated with different vehicle categories.

**Key Metrics:**

* Vehicle Risk Score
* High-Risk Customer Percentage
* Claim Frequency by Vehicle Type
* Average Vehicle Age

**Key Finding:**
SUV and Minivan owners consistently demonstrate higher insurance risk.

---

### 4. Root Cause Analysis

Identifies the key drivers behind insurance claims.

**Key Metrics:**

* Previous Claims vs Current Claim Amount
* Previous Claims vs Claim Frequency
* Travel Time vs Claim Frequency
* Vehicle Age vs Claim Amount

**Key Finding:**
Historical claims, travel exposure, and vehicle age are major contributors to future insurance risk.

---

### 5. Customer Demographics Analysis

Examines the relationship between customer demographics and insurance claims.

**Key Metrics:**

* Education vs Claim Amount
* Education vs Claim Frequency
* Kids Driving vs Claim Frequency
* Marital Status & Gender vs Claims

**Key Finding:**
High School and Bachelor's degree holders, along with unmarried customers, show higher claim activity.

---

## Calculated Fields Used

### Risk Score

```text
([CLM_AMT]/1000) + ([OLDCLAIM]/1000) + ([CLM_FREQ]*5)
```

Used to identify and rank high-risk customer segments.

---

### High-Risk Customer Flag

```text
IF [CLM_FREQ] >= 1
OR [OLDCLAIM] > 1000
THEN "High Risk"
ELSE "Low Risk"
END
```

Used to classify customers based on claim behavior and historical risk.

---

## Key Insights

1. Urban customers have a significantly higher history of previous claims compared to rural customers.
2. Urban customers generate higher average claim amounts than rural customers.
3. Blue-collar customers record the highest average claim amounts among all occupational groups.
4. Blue-collar customers rank highest in both Risk Score and High-Risk Customer percentage.
5. SUV and Minivan owners consistently rank among the highest in both Risk Score and High-Risk Customer percentage.
6. SUVs account for the highest number of claims compared to all other vehicle categories.
7. Customers with a history of previous claims tend to generate larger claim amounts in the future.
8. Longer travel times and older vehicles are associated with higher claim frequency and claim amounts.
9. Customers with High School and Bachelor's education levels exhibit higher claim amounts and claim frequencies compared to other education groups.
10. Unmarried customers, particularly unmarried women, demonstrate higher claim activity than their married counterparts.

---

## Business Recommendations

* Implement location-based premium pricing for urban policyholders.
* Strengthen underwriting policies for high-risk occupational groups.
* Introduce vehicle-specific premium adjustments for SUV and Minivan owners.
* Incorporate historical claim behavior into underwriting and renewal decisions.
* Consider travel exposure and vehicle age during premium calculation.
* Develop targeted customer education and risk awareness programs.
* Use demographic segmentation to personalize insurance offerings and improve customer retention.

---

## Business Impact

This analysis helps insurance companies:

* Improve risk assessment accuracy.
* Reduce claim losses through proactive risk management.
* Optimize premium pricing strategies.
* Identify high-risk customer segments.
* Support data-driven decision-making.

---

## Conclusion

The project demonstrates how data visualization and business intelligence techniques can be used to uncover key insurance risk drivers. By analyzing geographic, occupational, vehicle, behavioral, and demographic factors, insurers can make more informed decisions and develop effective strategies to improve profitability while managing risk.
