# SCT_DA_2 - Data Cleaning and Preparation

## Overview
This project focuses on cleaning and preparing the Global Superstore dataset using Python and Pandas. The dataset was analyzed for missing values, duplicate records, and data quality issues before being prepared for further analysis.

## Objective
The objective of this task was to:

- Load and inspect the dataset
- Identify missing values
- Check for duplicate records
- Clean the dataset
- Export the cleaned dataset for future analysis

## Dataset Information

- Dataset Name: Global Superstore
- Original File: Global Superstore.xls
- Total Records: 51,290
- Original Columns: 24

## Tools Used

- Python
- Pandas
- Jupyter Notebook
- Git
- GitHub

## Project Files

| File | Description |
|--------|------------|
| Global Superstore.xls | Original dataset |
| data_cleaning.ipynb | Jupyter Notebook containing the cleaning process |
| cleaned_global_superstore.csv | Cleaned dataset |

## Data Cleaning Process

### Step 1: Load Dataset

The dataset was loaded into a Jupyter Notebook using Pandas.

### Step 2: Explore Dataset

Initial exploration was performed using:

```python
df.head()
df.info()
```

### Step 3: Missing Value Analysis

Missing values were identified using:

```python
df.isnull().sum()
```

Result:
- Postal Code column contained 41,296 missing values.

### Step 4: Duplicate Check

Duplicate records were checked using:

```python
df.duplicated().sum()
```

Result:
- No duplicate rows found.

### Step 5: Data Cleaning

The Postal Code column was removed due to excessive missing values.

```python
df.drop('Postal Code', axis=1, inplace=True)
```

### Step 6: Validation

The dataset was rechecked to confirm:

- No missing values remained
- Dataset structure was maintained
- Duplicate records were removed

### Step 7: Export Cleaned Dataset

The cleaned dataset was exported as:

```python
cleaned_global_superstore.csv
```

## Results

### Before Cleaning

- Rows: 51,290
- Columns: 24
- Missing Values:
  - Postal Code: 41,296

### After Cleaning

- Rows: 51,290
- Columns: 23
- Missing Values: 0
- Duplicate Rows: 0

## Key Learnings

- Data inspection using Pandas
- Handling missing values
- Dataset validation techniques
- Data preprocessing workflow
- Exporting cleaned datasets
- Git and GitHub project management
## Screenshots

### Dataset Preview
![Dataset Preview](screenshots/Screenshot%202026-06-02%20004450.png)

### Dataset Information
![Dataset Information](screenshots/Screenshot%202026-06-02%20004517.png)

### Missing Values Before Cleaning
![Missing Values Before Cleaning](screenshots/Screenshot%202026-06-02%20004541.png)

### Cleaning Process
![Cleaning Process](screenshots/Screenshot%202026-06-02%20004651.png)

### Final Output
![Final Output](screenshots/Screenshot%202026-06-02%20004843.png)

## Repository Naming Convention

Repository Name:
SCT_DA_2

## Outcome

Successfully cleaned and prepared the Global Superstore dataset for future data analysis, visualization, and business intelligence tasks.
