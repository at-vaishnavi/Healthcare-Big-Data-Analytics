# Healthcare Big Data Analytics Using PySpark

## Project Overview

Healthcare organizations generate large amounts of data related to patients, hospital admissions, diagnoses, treatments, and billing. Analyzing this data can help identify healthcare trends, understand patient admission patterns, and gain insights into hospital operations.

This project uses **Apache PySpark** to process and analyze healthcare datasets. It focuses on data cleaning, distributed data processing, healthcare analytics, and hospital readmission analysis.

The project is implemented using Python and PySpark in a Jupyter Notebook environment.

## Objectives

- Understand and process large healthcare datasets using PySpark.
- Perform data cleaning and preprocessing.
- Analyze disease and diagnosis patterns.
- Calculate patient age statistics and hospital length of stay.
- Analyze hospital admissions by ward, hospital, and admission type.
- Identify 7-day and 30-day readmission patterns.
- Examine healthcare billing and government subsidy distribution.
- Use PySpark DataFrame operations and Spark SQL for analysis.

## Technologies Used

- **Programming Language:** Python
- **Big Data Processing:** Apache PySpark 3.5.6
- **Notebook Environment:** Jupyter Notebook
- **Data Processing:** PySpark DataFrames and Spark SQL
- **Development Environment:** Anaconda
- **Java:** JDK 17

## Dataset

The project uses the **India Hospital Readmission Dataset (2015–2024)**.

Source: [Kaggle – India Hospital Readmission Dataset](https://www.kaggle.com/datasets/digutlaranjithkumar/india-hospital-readmission-dataset-20152024)

The dataset contains five CSV files:

| Dataset | Description |
|---|---|
| patients.csv | Patient demographic and medical information |
| admissions.csv | Hospital admission and discharge details |
| diagnoses.csv | Patient diagnosis information |
| hospitals.csv | Hospital details and classifications |
| billing.csv | Hospital billing and cost information |

### Dataset Size

| Dataset | Number of Records |
|---|---:|
| Patients | 86,400 |
| Admissions | 120,000 |
| Diagnoses | 271,341 |
| Hospitals | 33 |
| Billing | 120,000 |

**Note:** The dataset is synthetic and is used for academic and analytical purposes.

## Project Workflow

1. **Spark Initialization:** Create a SparkSession to perform distributed data processing.
2. **Data Loading:** Load the five healthcare CSV datasets into PySpark DataFrames.
3. **Data Cleaning:** Check for missing values, duplicate records, and inconsistent categorical values.
4. **Data Preprocessing:** Prepare the datasets for analysis.
5. **Data Analysis:** Perform aggregations, grouping, filtering, and calculations using PySpark DataFrame operations.
6. **Spark SQL:** Execute SQL queries to analyze healthcare information.
7. **Result Interpretation:** Examine the results to identify healthcare trends and readmission patterns.

## Key Analysis Performed

- Disease category distribution.
- Patient age statistics.
- Average hospital length of stay.
- Hospital admissions by ward and admission type.
- Hospital-wise admission analysis.
- 7-day and 30-day readmission analysis.
- Readmission rates by ward, admission type, diagnosis category, age group, and previous admissions.
- Healthcare billing analysis, including government subsidies and out-of-pocket expenses.

## Key Findings

Some important observations from the analysis include:

- Cardiovascular diseases had the highest number of diagnosis records.
- The average patient age was approximately **48 years**.
- The average hospital stay was approximately **6.85 days**.
- The overall 30-day readmission rate was approximately **11.84%**.
- ICU admissions showed a higher 30-day readmission rate (approximately **23.76%**) compared with general ward admissions (approximately **7.90%**).
- Patients aged 60 and above showed a higher 30-day readmission rate than younger age groups.
- Patients with a greater number of previous admissions generally showed higher readmission rates.
- Government subsidies covered approximately **49.7%** of the average hospital billing cost.

These findings are based on the supplied synthetic dataset and should not be interpreted as conclusions about actual hospital populations.

## How to Run the Project

### Prerequisites

- Python
- Java JDK 17
- Apache PySpark 3.5.6
- Anaconda or Jupyter Notebook

### Installation

Install PySpark:

```bash
pip install pyspark==3.5.6
```

### Run the Notebook

1. Clone this repository:

```bash
git clone https://github.com/at-vaishnavi/Healthcare-Big-Data-Analytics.git
```

2. Navigate to the project directory:

```bash
cd Healthcare-Big-Data-Analytics
```

3. Download the dataset from the Kaggle source provided above.

4. Place the five CSV files inside a folder named `dataset` in the project directory.

5. Open Jupyter Notebook:

```bash
jupyter notebook
```

6. Open `Healthcare_Big_Data_Analytics.ipynb` and execute the cells in order.

**Note:** Update the dataset file paths in the notebook according to your local folder location before execution.

## Future Enhancements

- Develop interactive healthcare analytics dashboards.
- Explore machine learning techniques for readmission prediction using Spark MLlib.
- Extend the analysis with additional healthcare performance indicators.


---

*Academic project developed to explore big data processing and healthcare analytics using Apache PySpark.*
