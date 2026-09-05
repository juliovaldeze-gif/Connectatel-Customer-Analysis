# 📊 ConnectaTel - Customer Analysis and Usage Patterns

## 📌 Project Objective

The objective of this project is to analyze the behavior of ConnectaTel customers, a telecommunications company operating in Latin America, using customer and service usage data recorded during 2024.

Through data cleaning, exploration, and analysis techniques, the project aims to identify usage patterns, customer segments, and business opportunities that can help optimize service plan offerings and improve decision-making.

---

## 📂 Datasets Used

### users_latam.csv

Contains customer demographic information:

* user_id
* age
* city
* plan
* signup_date

### usage.csv

Contains service usage records:

* id
* user_id
* type (call or text)
* duration
* event_date

### plans.csv

Contains information about the service plans offered by ConnectaTel:

* plan_name
* messages_included
* gb_per_month
* minutes_included
* usd_monthly_pay
* usd_per_gb
* usd_per_message
* usd_per_minute

---

## 🔎 Analysis Stages

### 1. Exploratory Data Analysis (EDA)

* Review of dataset structure.
* Validation of data types.
* Identification of missing values.
* Initial descriptive analysis.

### 2. Data Cleaning

* Correction of invalid values and sentinel values.
* Treatment of missing values.
* Standardization of city names.
* Conversion of dates to the appropriate format.
* Validation of customer age ranges.

### 3. Data Integration

* Consolidation of customer and usage information.
* Creation of the analytical dataset `user_profile`.

### 4. Usage Analysis

* Calculation of messages sent per user.
* Calculation of calls made per user.
* Calculation of total minutes used.
* Generation of histograms and descriptive statistics.

### 5. Outlier Detection

* Creation of boxplots.
* Identification of outliers using the IQR method.
* Evaluation of the impact of high-usage customers.

### 6. Customer Segmentation

* Segmentation by age group:
  * Young
  * Adult
  * Senior

* Segmentation by usage level:
  * Low Usage
  * Medium Usage
  * High Usage

### 7. Executive Analysis

* Identification of high-value customers.
* Detection of usage patterns.
* Development of recommendations for new service plans and commercial strategies.

---

## 🚀 How to Run the Project

### Option 1: Google Colab

1. Download the `.ipynb` file.
2. Open Google Colab.
3. Select **File → Upload Notebook**.
4. Upload the project notebook.
5. Upload the required CSV files.
6. Run the cells in order.

### Option 2: Jupyter Notebook

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook
```

Open the notebook and run all cells sequentially.

---

## 📋 Reproduction Guide

1. Load the datasets.
2. Explore data quality.
3. Correct missing values and inconsistencies.
4. Create aggregated usage variables for each user.
5. Generate histograms and boxplots.
6. Identify outliers using the IQR method.
7. Create customer segments based on age and usage level.
8. Analyze the results and develop business recommendations.

---

## 🛠️ Technologies Used

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Jupyter Notebook

---

## 🎯 Key Findings

* Most customers belong to the medium-usage segment.
* Customers with usage levels significantly above the average were identified.
* High-usage customers represent an opportunity for premium plans and customer retention strategies.
* Segmentation by age and usage level helps identify opportunities for more personalized service offerings.
