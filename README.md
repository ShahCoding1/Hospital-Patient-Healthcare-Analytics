# 🏥 Hospital Patient & Healthcare Analytics

## 📊 Project Overview

This project is an **end-to-end healthcare data analytics project** developed using Python, Pandas, NumPy, Matplotlib, Seaborn, and SciPy.

The goal of this project is to analyze hospital patient data and discover meaningful patterns related to **patient demographics, medical conditions, hospital admissions, length of stay, billing amounts, insurance providers, medications, and test results**.

The project demonstrates how healthcare data can be transformed from raw records into meaningful **statistical insights and visual analytics** that can support healthcare management and operational decision-making.

---

## 🎯 Objectives

The main objectives of this project are to:

* Analyze patient demographics and age distribution.
* Identify the most common medical conditions.
* Analyze hospital admission types.
* Examine patient length of stay.
* Analyze hospital billing amounts.
* Compare billing across medical conditions and admission types.
* Analyze insurance providers and healthcare costs.
* Explore medication usage.
* Analyze patient test results.
* Identify relationships between patient characteristics and healthcare outcomes.
* Perform statistical hypothesis testing using Chi-Square tests and t-tests.
* Generate actionable healthcare management insights.

---

## 📁 Dataset

The dataset contains hospital patient records with the following variables:

| Column               | Description                           |
| -------------------- | ------------------------------------- |
| `Age`                | Patient age                           |
| `Gender`             | Patient gender                        |
| `Medical Condition`  | Patient's diagnosed medical condition |
| `Date of Admission`  | Date when the patient was admitted    |
| `Hospital`           | Hospital associated with the patient  |
| `Insurance Provider` | Patient's insurance provider          |
| `Billing Amount`     | Total hospital billing amount         |
| `Admission Type`     | Type of hospital admission            |
| `Discharge Date`     | Date when the patient was discharged  |
| `Medication`         | Medication prescribed to the patient  |
| `Test Results`       | Patient's test result category        |

---

## 🛠️ Technologies & Tools

### Programming Language

* Python

### Libraries

* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy

### Environment

* Google Colab
* Jupyter Notebook

### Version Control

* Git
* GitHub

---

## 🔄 Project Workflow

The project follows a complete data analytics workflow:

```text
Raw Healthcare Dataset
        ↓
Data Loading
        ↓
Data Inspection
        ↓
Data Cleaning
        ↓
Feature Engineering
        ↓
Exploratory Data Analysis
        ↓
Statistical Analysis
        ↓
Data Visualization
        ↓
Healthcare Insights
        ↓
Management Recommendations
```

---

## 🧹 Data Cleaning & Preparation

The following preprocessing steps were performed:

* Checked dataset dimensions.
* Inspected data types.
* Identified missing values.
* Checked duplicate records.
* Removed duplicate records.
* Converted admission and discharge dates into datetime format.
* Converted age and billing amount into numeric values.
* Removed unnecessary whitespace from categorical values.
* Created a new **Length of Stay** variable.
* Checked for invalid or negative stay durations.
* Performed final data-quality validation.

### Feature Engineering

A new variable was created:

```text
Length of Stay = Discharge Date - Date of Admission
```

This feature allows the analysis of hospital utilization and patient stay duration.

---

# 📊 Exploratory Data Analysis

## 👥 Patient Demographics

The project analyzes:

* Patient age distribution
* Gender distribution
* Age groups
* Medical conditions by gender

Age groups were created to make demographic analysis easier:

```text
0–18
19–30
31–45
46–60
61+
```

---

## 🏥 Medical Condition Analysis

The project identifies:

* Most common medical conditions
* Number of patients by condition
* Medical conditions by gender
* Average billing by medical condition
* Average length of stay by medical condition
* Relationship between medical conditions and medications
* Relationship between medical conditions and test results

---

## 🚑 Admission Analysis

Different admission types are analyzed to understand hospital utilization.

The analysis includes:

* Admission type distribution
* Admission type percentages
* Admission trends over time
* Length of stay by admission type
* Billing amount by admission type
* Relationship between admission type and medical condition
* Relationship between admission type and test results

---

## 📅 Admission Trends

Admission dates are used to identify changes in patient volume over time.

The project analyzes:

* Monthly admission trends
* Patient volume over time
* Changes in admission patterns

This can help identify periods with relatively higher or lower hospital utilization.

---

## ⏱️ Length of Stay Analysis

Patient length of stay is calculated using admission and discharge dates.

The analysis includes:

* Distribution of length of stay
* Average length of stay
* Median length of stay
* Length of stay by admission type
* Length of stay by medical condition
* Relationship between length of stay and billing amount

---

## 💰 Healthcare Billing Analysis

The project examines hospital billing patterns.

Analysis includes:

* Billing amount distribution
* Average billing amount
* Median billing amount
* Total billing amount
* Billing by medical condition
* Billing by admission type
* Billing by insurance provider
* Relationship between length of stay and billing
* Relationship between age and billing

---

## 🏦 Insurance Provider Analysis

Insurance providers are analyzed based on:

* Number of patients
* Average billing amount
* Relationship with admission types

This helps explore differences in healthcare utilization and billing across insurance groups.

---

## 💊 Medication Analysis

The project analyzes medication usage across patients.

Analysis includes:

* Most frequently used medications
* Medication distribution
* Medication by medical condition

A heatmap is used to visualize the relationship between medical conditions and medications.

---

## 🧪 Test Results Analysis

Patient test results are analyzed to understand their distribution across the dataset.

The project examines:

* Test result categories
* Test results by medical condition
* Test results by gender
* Test results by admission type

---

# 📈 Statistical Analysis

Statistical tests were included to move beyond simple descriptive analysis.

## Chi-Square Test

Chi-Square tests were performed to examine relationships between categorical variables.

Examples include:

* Gender vs Medical Condition
* Gender vs Test Results
* Admission Type vs Test Results
* Admission Type vs Medical Condition
* Insurance Provider vs Admission Type
* Medical Condition vs Medication

### Hypotheses

For each Chi-Square test:

**H₀:** There is no significant association between the two categorical variables.

**H₁:** There is a significant association between the two categorical variables.

A significance level of:

```text
α = 0.05
```

was used.

---

## Independent T-Test

An independent t-test is used to compare billing amounts between two admission groups when the dataset contains exactly two admission categories.

### Hypotheses

**H₀:** The mean billing amounts are equal between the groups.

**H₁:** The mean billing amounts are different between the groups.

---

# 📊 Correlation Analysis

Correlation analysis was performed for numerical variables including:

* Age
* Billing Amount
* Length of Stay

The project examines:

```text
Age ↔ Billing Amount
Length of Stay ↔ Billing Amount
```

A correlation matrix and scatter plots are used to visualize these relationships.

---

# 📉 Visualizations

The project generates several visualizations, including:

* Patient age distribution
* Gender distribution
* Medical condition distribution
* Admission type distribution
* Monthly admission trend
* Length of stay distribution
* Billing distribution
* Billing by medical condition
* Billing by admission type
* Insurance provider analysis
* Medication distribution
* Medical condition vs medication heatmap
* Test results distribution
* Medical condition vs test results heatmap
* Age vs billing scatter plot
* Length of stay vs billing scatter plot
* Correlation matrix

---

# 🔎 Key Findings

The notebook automatically identifies important findings from the dataset, including:

* Most common medical condition
* Most common admission type
* Most common medication
* Most common test result
* Medical condition with the highest average billing
* Insurance provider with the highest average billing
* Medical condition with the longest average hospital stay
* Correlation between age and billing
* Correlation between length of stay and billing

> **Note:** Exact numerical findings should be taken from the final notebook output after running the analysis on the dataset.

---

# 💡 Healthcare Analytics Insights

The analysis can provide insights into several important healthcare management areas:

### 1. Patient Demographics

Understanding patient age and gender distributions can help hospitals understand their patient population.

### 2. Medical Conditions

Identifying frequently occurring conditions can help healthcare organizations understand the major categories of patient demand represented in the dataset.

### 3. Hospital Utilization

Admission types and length of stay provide information about how hospital resources are being utilized.

### 4. Healthcare Costs

Billing analysis can help identify conditions, admission types, or insurance groups associated with higher healthcare costs.

### 5. Medication Patterns

Analyzing medication usage alongside medical conditions can reveal treatment patterns within the dataset.

### 6. Test Results

Test-result analysis can help identify patterns across patient groups, medical conditions, and admission types.

---

# 📌 Recommendations

Based on the analytical framework, healthcare organizations could consider:

* Monitoring conditions associated with higher average costs.
* Reviewing patients or conditions associated with longer hospital stays.
* Monitoring monthly admission patterns for resource planning.
* Comparing healthcare costs across admission categories.
* Using patient demographic information for better resource planning.
* Monitoring medication utilization patterns.
* Using statistical testing before making conclusions about relationships between variables.
* Developing interactive dashboards for continuous healthcare monitoring.

---

# ⚠️ Limitations

This project has several limitations:

* The dataset represents historical patient records rather than live hospital data.
* The analysis is observational and does not establish causation.
* Statistical relationships should not automatically be interpreted as causal relationships.
* The dataset may not represent every hospital or healthcare system.
* Some potentially important clinical variables may not be available.
* Test-result categories provide limited clinical detail.
* Billing amounts may depend on factors that are not included in the dataset.

Therefore, the findings should be interpreted as **data analytics insights rather than clinical recommendations**.

---

# 🗂️ Project Structure

```text
Hospital-Patient-Healthcare-Analytics/
│
├── Hospital_Patient_Healthcare_Analytics.ipynb
│
├── hospital_healthcare_cleaned.csv
│
├── README.md
│
└── images/
    ├── patient_age_distribution.png
    ├── medical_conditions.png
    ├── admission_types.png
    ├── admission_trend.png
    ├── length_of_stay.png
    ├── billing_analysis.png
    ├── insurance_analysis.png
    ├── test_results.png
    └── correlation_matrix.png
```

---

# 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/ShahCoding1/Hospital-Patient-Healthcare-Analytics.git
```

### 2. Open Google Colab

Upload:

```text
Hospital_Patient_Healthcare_Analytics.ipynb
```

### 3. Upload the dataset

When prompted by the notebook, upload the healthcare CSV dataset.

### 4. Run the notebook

Execute the cells from top to bottom.

The notebook will:

* Load the dataset
* Clean the data
* Perform exploratory analysis
* Generate visualizations
* Perform statistical tests
* Generate healthcare insights
* Export the cleaned dataset

---

# 📦 Output

The project produces:

* Cleaned healthcare dataset
* Statistical summaries
* Healthcare KPIs
* Exploratory visualizations
* Correlation analysis
* Chi-Square test results
* T-test results
* Automated key findings
* Healthcare management recommendations

---

# 🧠 Skills Demonstrated

This project demonstrates practical skills in:

* Data Cleaning
* Data Preprocessing
* Exploratory Data Analysis (EDA)
* Feature Engineering
* Descriptive Statistics
* Inferential Statistics
* Hypothesis Testing
* Chi-Square Testing
* T-Tests
* Correlation Analysis
* Data Visualization
* Healthcare Analytics
* Business/Management Insights
* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* SciPy
* Google Colab
* GitHub

---

# 🏁 Conclusion

This project demonstrates an end-to-end approach to **healthcare data analytics**, starting from raw patient records and progressing through data cleaning, exploratory analysis, visualization, statistical testing, and insight generation.

The analysis provides a structured view of **patient demographics, medical conditions, admissions, hospital stays, billing, insurance, medications, and test results**.

It also demonstrates how Python-based analytics can be used to transform healthcare data into understandable insights that can support **data-driven operational and management decisions**.

---

## 👨‍💻 Author

**Muhammad Shah Khalid**

**Software Engineer | AI/ML & Data Science | Web Development**

### Technologies

```text
Python • Pandas • NumPy • SciPy • Matplotlib • Seaborn
React • Node.js • Express • MongoDB • Git • GitHub
```

---

⭐ If you find this project useful, consider giving the repository a star!
