# 🚲 Bike Sales Analysis & Excel Dashboard

## 📌 Project Overview

This project demonstrates an end-to-end **data analysis workflow using Microsoft Excel**, from raw data preparation and data cleaning to exploratory analysis, visualization and dashboard development.

The objective was to analyze customer demographic and purchasing data to understand **which customer characteristics and behaviors are associated with bicycle purchases** and present the findings through an interactive Excel dashboard.

The project focuses on demonstrating practical data analyst skills including:

- Data cleaning and preparation
- Data transformation
- Exploratory data analysis
- Conditional logic using Excel formulas
- Pivot Tables and Pivot Charts
- Interactive dashboard development
- Identifying patterns and business insights
- Communicating findings through data visualization

---

## 🎯 Business Objective

The goal of this analysis is to understand **customer purchasing behavior** and identify characteristics that may help a bike retailer better understand its customers.

The analysis explores the following questions:

- How does income differ between customers who purchased a bike and those who did not?
- Does age appear to influence bike purchasing behavior?
- Is there a relationship between commute distance and bike purchases?
- How does purchasing behavior vary across gender, marital status, education and region?
- Which customer segments appear more likely to purchase a bike?
- How can these insights support more targeted marketing and customer segmentation?

---

## 🗂️ Dataset

The dataset contains customer-level information, including demographic, financial and behavioral attributes.

### Key Variables

| Category | Variables |
|---|---|
| Demographics | Gender, Age, Marital Status |
| Socioeconomic | Income, Education |
| Location | Region |
| Behavior | Commute Distance |
| Outcome | Purchased Bike |
| Derived Variable | Age Bracket |

The **Purchased Bike** field serves as the primary outcome variable for understanding customer purchasing behavior.

---

# 🔄 Data Analysis Workflow

The project followed a structured data analysis process.

### 1. Data Preparation

I began by creating a working copy of the original dataset to preserve the raw data and avoid modifying the source data directly.

The initial preparation included:

- Creating a separate working dataset
- Reviewing the structure and consistency of the data
- Removing duplicate records
- Correcting inappropriate or inconsistent data types
- Checking categorical fields for consistency
- Preparing the dataset for analysis

This ensured that the data used for analysis was structured and suitable for further transformation.

---

### 2. Data Transformation

To make the analysis more meaningful, I created an **Age Bracket** variable using Excel `IF` statements.

Customers were grouped into age categories:

- Adolescent
- Middle Age
- Old

This transformation allowed me to move beyond analyzing individual ages and instead identify broader customer segments.

#### Example Excel Logic

```excel
=IF(Age<31,"Adolescent",IF(Age<55,"Middle Age","Old"))

The exact thresholds can be adjusted depending on the analytical definition used.
```
---

### 3. Exploratory Data Analysis

I used **Pivot Tables** to aggregate and analyze the data across different customer characteristics.

The analysis examined:

- Average income
- Bike purchase counts
- Age brackets
- Gender
- Commute distance
- Region
- Marital status
- Education level

Pivot Tables were used to identify patterns and relationships before converting the results into visualizations.

### 4. Data Visualization

I created **Pivot Charts** from the analytical summaries to communicate the key patterns visually.

The dashboard includes visualizations showing:

**1. Average Income by Gender & Bike Purchase**

This visualization compares the average income of customers who purchased a bike with those who did not, segmented by gender.

**2. Purchases by Customer Age Bracket**

This visualization examines bike purchasing behavior across different age groups.

**3. Customer Commute Distance**

This visualization compares bike purchases against customers' commute distances.

These visualizations were selected to answer the key business questions while keeping the dashboard focused and easy to interpret.

--- 

### 📊 Interactive Dashboard

The final analysis was presented through an interactive Bike Sales Dashboard built entirely in Microsoft Excel.

The dashboard allows users to filter the analysis using:

- Marital Status
- Region
- Education

These slicers allow users to explore how purchasing behavior changes across different customer segments.
---

### 🔎 Key Insights

The analysis revealed several patterns in customer purchasing behavior.

**1. Income appears to be associated with purchasing behavior**

Customers who purchased bikes generally show different average income levels compared with customers who did not purchase, with the relationship varying by gender.

This suggests that income may be a useful variable for customer segmentation and marketing targeting.

**2. Age is an important customer characteristic**

The analysis shows differences in purchasing behavior across age brackets, with the middle-age segment representing a particularly important customer group.

This suggests that marketing strategies could be tailored according to different age segments.

**3. Commute distance shows different purchasing patterns**

Bike purchasing behavior varies across commute-distance categories.

Customers with shorter and moderate commutes display different purchase patterns compared with customers travelling longer distances, suggesting that commuting behavior may provide useful insight into potential bike demand.

**4. Customer characteristics can be explored through segmentation**

The dashboard's slicers make it possible to investigate how purchasing behavior changes across regions, education levels and marital status.

This demonstrates the value of interactive dashboards for moving from broad analysis to more targeted customer questions.
---


### 💡 Business Recommendations

Based on the analysis, a bike retailer could consider:

**🎯1. Segment customers by demographic characteristics**

Use age, gender, income, education and marital status to develop more targeted customer segments rather than using a one-size-fits-all marketing strategy.

**📍2. Develop region-specific campaigns**

Differences across regions can be explored through the dashboard to identify areas where bike purchasing behavior is stronger or weaker.

**🚴3. Target customers based on commuting behavior**

Commute distance can be used as a potential indicator of customer needs and purchasing intent. Marketing messages could emphasize different bike benefits depending on commuting patterns.

**💰4. Use income as part of customer segmentation**

Income differences between purchasers and non-purchasers could help inform product positioning, promotions and customer targeting.

---


### 🛠️ Tools & Techniques
**Tools**
- Microsoft Excel
- Pivot Tables
- Pivot Charts
- Excel Slicers
- Excel formulas

**Techniques**
- Data cleaning
- Duplicate removal
- Data type correction
- Data transformation
- Conditional logic
- Customer segmentation
- Exploratory data analysis
- Aggregation
- Data visualization
- Dashboard development
---

### 📁 Project Structure
```text
Bike-Sales-Analysis/
│
├── data/
│   ├── processed/
│   │   └── Final Dashboard.xlsx
│   │
│   └── raw/
│       └── Bike Purchases Datasets.xlsx
│
├── Visualization/
│   └── Dashboard.png
│
└── README.md
```
