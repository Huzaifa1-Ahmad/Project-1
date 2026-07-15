# 🧹 Project 1: Data Cleaning & Preparation

## 📌 Internship Information

**Organization:** DecodeLabs  
**Internship Program:** Data Analytics Industrial Training  
**Project:** Project 1 – Data Cleaning & Preparation  
**Intern:** Huzaifa Ahmad

---

# 📖 Project Overview

This project focuses on cleaning and preparing a raw Excel dataset using Python and the Pandas library.

The objective is to transform raw, inconsistent data into a clean and reliable dataset that can be used for reporting, dashboard creation, and future data analysis.

The project follows industry-standard data cleaning practices and ensures that the dataset is accurate, complete, and ready for business intelligence tools such as Power BI.

---

# 🎯 Project Objectives

The main objectives of this project are:

- Load the raw Excel dataset
- Understand the dataset structure
- Identify missing values
- Handle missing or null values
- Remove duplicate records
- Verify unique Order IDs
- Correct incorrect data types
- Standardize date formats
- Clean text columns
- Validate the cleaned dataset
- Export the cleaned Excel file

---

# 🛠 Technologies Used

- Python 3.13
- Pandas
- NumPy
- OpenPyXL
- Jupyter Notebook
- Visual Studio Code (VS Code)

---

# 📂 Project Structure

```
Project File
│
├── Data
│   └── Dataset for Data Analytics.xlsx
│
├── Cleaned_Data
│   └── Cleaned_Data.xlsx
│
├── notebook.ipynb
│
├── README.md
│
├── requirements.txt
│
└── virtual/
```

---

# 📊 Dataset Description

The dataset contains order-related information including:

- Order ID
- Order Date
- Customer ID
- Product
- Quantity
- Unit Price
- Shipping Address
- Payment Method
- Order Status
- Tracking Number
- Shipping Cost
- Delivery Date
- Customer Rating
- Total Price

---

# 🔄 Data Cleaning Process

The following data cleaning steps were performed:

## 1. Import Libraries

Imported all required Python libraries.

- Pandas
- NumPy

---

## 2. Load Dataset

Loaded the Excel dataset into a Pandas DataFrame.

---

## 3. Dataset Inspection

Performed an initial analysis using:

- df.head()
- df.shape
- df.columns
- df.info()
- df.describe()

---

## 4. Missing Value Analysis

Checked all columns for missing values.

```python
df.isnull().sum()
```

Handled missing values where required.

---

## 5. Duplicate Record Detection

Checked duplicate rows.

```python
df.duplicated().sum()
```

Removed duplicate records.

---

## 6. Duplicate Order ID Validation

Verified OrderID uniqueness.

```python
df["OrderID"].duplicated().sum()
```

Removed duplicate Order IDs if found.

---

## 7. Data Type Validation

Verified the correct data types for:

- Date
- Quantity
- Unit Price
- Shipping Cost
- Total Price

Converted incorrect data types where necessary.

---

## 8. Date Formatting

Validated and standardized all date fields.

---

## 9. Text Cleaning

Cleaned text columns by:

- Removing extra spaces
- Standardizing formatting
- Ensuring consistency

---

## 10. Final Data Validation

Performed final quality checks.

Verified:

- No missing values
- No duplicate rows
- No duplicate Order IDs
- Correct data types
- Correct date format

---

## 11. Export Clean Dataset

Saved the cleaned dataset.

```python
df.to_excel(
    "Cleaned_Data/Cleaned_Data.xlsx",
    index=False
)
```

---

# 📈 Project Workflow

```
Raw Excel Dataset
        │
        ▼
Load Dataset
        │
        ▼
Dataset Inspection
        │
        ▼
Missing Value Analysis
        │
        ▼
Duplicate Removal
        │
        ▼
Data Type Correction
        │
        ▼
Text Cleaning
        │
        ▼
Data Validation
        │
        ▼
Export Clean Dataset
```

---

# ✅ Project Outcome

After completing this project:

- Dataset successfully cleaned
- Missing values handled
- Duplicate records removed
- Duplicate Order IDs verified
- Date formats standardized
- Data types corrected
- Clean dataset exported successfully

The cleaned dataset is now ready for:

- Power BI Dashboards
- Data Visualization
- Business Intelligence
- Exploratory Data Analysis (EDA)
- Machine Learning Projects

---

# 📚 Skills Demonstrated

This project demonstrates practical knowledge of:

- Data Cleaning
- Data Preparation
- Data Validation
- Python Programming
- Pandas
- NumPy
- Excel Data Processing
- Jupyter Notebook
- Data Quality Management

---

# 📁 Output Files

```
Raw Dataset

Data/
└── Dataset for Data Analytics.xlsx

Clean Dataset

Cleaned_Data/
└── Cleaned_Data.xlsx
```

---

# 🚀 Future Work

The cleaned dataset will be used to build an interactive Power BI dashboard, including:

- Sales Overview
- Revenue Analysis
- Product Performance
- Customer Insights
- Order Status Analysis
- Payment Method Analysis
- Shipping Performance

---

# 👨‍💻 Author

**Huzaifa Ahmad**

BS Computer Science Student

Data Analytics Intern

DecodeLabs Industrial Training Program

---

# 🙏 Acknowledgements

Special thanks to **DecodeLabs** for providing the opportunity to work on real-world data analytics projects and gain hands-on experience in data cleaning, preparation, and business intelligence.