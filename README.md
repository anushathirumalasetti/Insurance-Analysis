
# 📊 Power BI Insurance Dashboard – Prism Insurance Pvt. Ltd.

## 📌 Project Overview

This project presents an **end-to-end Power BI Insurance Analytics Dashboard** built using transactional insurance data. The dashboard enables business stakeholders to monitor **premiums, coverage, claims, policy status, and customer demographics** through interactive visuals and KPIs.

The solution demonstrates strong capabilities in **data ingestion, data cleaning, data modeling, DAX, and dashboard design**, following industry best practices.

---

## 🏢 Business Context

Insurance companies require real-time insights into:

* Revenue from premiums
* Risk exposure via coverage amounts
* Claims performance and settlement efficiency
* Active vs inactive policies
* Customer and demographic trends

This dashboard helps decision-makers **identify high-performing policy types, monitor claim outcomes, and optimize operations**.

---

## 🗂️ Dataset Description

* **Source:** Insurance transactional CSV file
* **Data Includes:**

  * Policy details
  * Customer information
  * Premium amount
  * Coverage amount
  * Claim amount
  * Claim status (Rejected, Settled, Pending)
  * Policy status (Active / Inactive)
  * Demographic attributes (Gender, Age Group)

---

## 🧹 Data Cleaning & Transformation (Power Query)

The following steps were performed in **Power Query Editor**:

1. Removed duplicate records using **PolicyNumber** and **ClaimNumber**
2. Handled null and missing values in:

   * PremiumAmount
   * CoverageAmount
   * ClaimAmount
3. Converted data types:

   * Dates
   * Numeric fields
   * Text fields
4. Standardized categorical values:

   * Policy types
   * Claim status values
5. Filtered invalid and incomplete records to ensure data quality

---

## 🧩 Data Modeling

* Created relationships between:

  * **Policy Table**
  * **Customer Table**
  * **Claim Table**
* Implemented a **Star Schema** model:

  * Fact table for claims
  * Dimension tables for policy and customer
* Optimized for:

  * Performance
  * Accurate aggregations
  * Scalable reporting

---

## 🧮 DAX Measures Used

Key DAX measures created:

```DAX
Total Premium Amount = SUM(PremiumAmount)

Total Coverage Amount = SUM(CoverageAmount)

Total Claim Amount = SUM(ClaimAmount)

Active Policy Count =
CALCULATE(COUNT(PolicyNumber), PolicyStatus = "Active")

Inactive Policy Count =
CALCULATE(COUNT(PolicyNumber), PolicyStatus = "Inactive")
```

Additional measures were created for:

* Claim status counts (Rejected, Settled, Pending)
* Policy-wise claim totals

---

## 📈 Dashboard Features

### 🔹 KPI Cards

* Total Premium Amount
* Total Coverage Amount
* Total Claim Amount

### 🔹 Visualizations

* **Bar Chart:** Premium Amount by Policy Type
* **Donut Chart:** Active vs Inactive Policies
* **Column Chart:** Number of Claims by Claim Status
* **Line Chart:** Claim Amount by Age Group
* **Table:** Policy-wise Claim Financial Breakdown

### 🔹 Slicers

* Policy Number
* Claim Number
* Customer ID

These slicers allow users to **drill down into specific policies or customers** dynamically.

---

## 💡 Business Insights Enabled

* Identify **high-revenue policy types** (e.g., Travel, Health)
* Monitor **claims settlement efficiency**
* Analyze **risk exposure** through coverage vs claims
* Understand **customer demographics and behavior**
* Track **policy lifecycle (Active vs Inactive)**

---

## 🛠️ Tools & Technologies

* **Power BI Desktop**
* **Power Query**
* **DAX**
* **CSV Data Source**
* **Data Modeling (Star Schema)**

---

## 🎯 Key Skills Demonstrated

* Data Cleaning & Transformation
* Data Modeling & Relationships
* DAX Calculations
* Dashboard Design & UX
* Business Insight Generation
* End-to-End BI Development

---

## 📌 Conclusion

This project showcases a complete **Business Intelligence lifecycle**, from raw data ingestion to an interactive executive dashboard. It highlights strong proficiency in **Power BI, analytics, and data-driven storytelling**, making it suitable for **Data Analyst, Business Analyst, and BI Developer roles**.

---

## 📎 Preview
<img width="1302" height="737" alt="image" src="https://github.com/user-attachments/assets/52d2fb31-69f6-47ff-8d62-93ed48a42578" />




---


