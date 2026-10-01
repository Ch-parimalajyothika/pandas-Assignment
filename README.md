# 📊 Pandas Assignment – Data Analysis & Data Cleaning

## 📌 Overview

This repository contains my **Pandas Assignment**, implemented using **Python, Pandas, and NumPy** in a Jupyter Notebook.

The assignment demonstrates fundamental and practical concepts of Pandas, including **Series and DataFrames, data selection, filtering, statistical analysis, correlation analysis, CSV processing, missing-value handling, duplicate detection, data validation, and real-world data cleaning**.

The notebook contains the assignment questions, Python code, executed outputs, and explanations for the completed tasks.

---

## 🎯 Objectives

The main objectives of this assignment are to:

- Understand and work with Pandas Series and DataFrames
- Perform data selection, filtering, and manipulation
- Apply statistical operations and analysis
- Perform correlation analysis
- Read and process CSV datasets
- Handle missing and inconsistent data
- Identify and remove duplicate records
- Detect invalid values
- Convert and clean inconsistent data values
- Perform practical data-cleaning operations
- Understand the importance of data validation before analysis

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Programming language |
| **Pandas** | Data manipulation and analysis |
| **NumPy** | Numerical operations |
| **Jupyter Notebook** | Interactive notebook environment |
| **Visual Studio Code** | Development environment |

---

# 📚 Assignment Contents

The assignment is divided into **four sections: A, B, C, and D**.

---

## 🔹 Section A – Pandas Fundamentals

This section covers fundamental Pandas concepts and operations.

### Topics Covered

- Pandas Series
- Pandas DataFrames
- Creating Series and DataFrames
- Accessing DataFrame elements
- Data selection
- Statistical operations
- Grouping and analysis
- Correlation analysis

This section demonstrates how Pandas can be used to represent, access, manipulate, and analyze structured data.

---

## 🔹 Section B – Pandas Operations

This section focuses on commonly used Pandas operations.

### Topics Covered

- Reading CSV files
- Sorting DataFrames
- Handling missing values
- Working with DataFrame columns
- Updating DataFrame values
- Calculating correlation between columns

These operations demonstrate practical techniques for manipulating and analyzing tabular data.

---

## 🔹 Section C – Practical Data Analysis

This section demonstrates practical data-analysis techniques using Pandas and NumPy.

### Topics Covered

- Broadcasting
- CSV data processing
- Inspecting unique values
- Handling missing values
- Date conversion
- Data type handling
- Mean calculation
- Median calculation
- Identifying extreme values
- Finding maximum values
- Investigating unusual data values

The section also demonstrates how different statistical measures can provide different interpretations of a dataset.

---

# 🔹 Section D – Data Cleaning

Section D focuses on cleaning a deliberately inconsistent student-assessment dataset.

### Data Cleaning Tasks

- Inspecting the dataset using `head()`, `info()`, and `isnull().sum()`
- Standardizing inconsistent department names
- Removing exact duplicate records
- Handling `Absent`, `NA`, and blank values
- Distinguishing between **Absent** and **Not Entered**
- Extracting numeric values from entries such as `"88 marks"`
- Identifying values outside the valid `0–100` range
- Handling invalid marks
- Displaying the final cleaned DataFrame
- Reporting records removed and invalid values identified

---

# 🧹 Data Cleaning Workflow

The data-cleaning process follows a structured workflow:

```text
Load Data
    ↓
Inspect Data
    ↓
Standardize Data
    ↓
Remove Duplicates
    ↓
Handle Missing Values
    ↓
Convert & Clean Values
    ↓
Validate Data
    ↓
Handle Invalid Values
    ↓
Generate Clean Data
```

This workflow demonstrates how raw and inconsistent data can be systematically processed before performing analysis.

---

## 1. Data Inspection

The dataset is first inspected to understand its structure, columns, data types, and missing values.

The following Pandas operations are used:

```python
df.head()
df.info()
df.isnull().sum()
```

These operations help identify the initial condition of the dataset before cleaning.

---

## 2. Standardizing Department Names

The dataset contains inconsistent representations of department names.

For example:

```text
IT
it
I.T.
```

These values are standardized into:

```text
IT
```

Similarly:

```text
Finance
finance
```

are standardized into:

```text
Finance
```

This ensures that the same department is represented consistently throughout the dataset.

---

## 3. Removing Duplicate Records

The dataset contains an exact duplicate record.

Duplicate records are identified and removed so that the same student record does not appear more than once.

The number of duplicate records removed is also reported in the notebook.

---

## 4. Handling Missing Values

The dataset contains different types of missing or incomplete marks information, including:

```text
Absent
NA
Blank values
```

These values are not automatically treated as the same condition.

The cleaning process distinguishes between:

- **Absent** – the student was absent
- **Not Entered** – the mark has not been entered

This distinction helps preserve the meaning of the original data.

### Why should missing values be investigated before deletion?

Missing values should be investigated before deleting them because different missing values may have different meanings.

For example, an `Absent` student and a student whose mark has not yet been entered are not necessarily the same situation.

Deleting missing records without investigation may result in:

- Loss of valid information
- Reduced dataset size
- Potential bias in analysis

---

## 5. Converting Inconsistent Mark Values

Some marks contain text along with the numeric value.

For example:

```text
88 marks
```

is processed to obtain:

```text
88
```

This allows the value to be converted into a numeric format and used for further analysis.

---

## 6. Validating Marks

The valid range for marks is:

```text
0 – 100
```

The dataset is checked for values outside this range.

For example:

```text
105
```

is identified as an invalid mark because it is greater than `100`.

Invalid values are identified and handled separately instead of being treated as valid marks.

---

## 7. Final Cleaned Data

After completing the cleaning operations, the final DataFrame is displayed.

The notebook also reports:

- Number of duplicate records removed
- Number of missing marks remaining
- Number of invalid marks identified

This provides a summary of the data-cleaning process.

---

# 📊 Data-Cleaning Summary

| Data Issue | Example | Handling |
|---|---|---|
| Inconsistent department | `IT`, `it`, `I.T.` | Standardized |
| Duplicate record | Repeated student record | Removed |
| Absent student | `Absent` | Preserved as status |
| Missing entry | Blank / `NA` | Treated as missing / not entered |
| Text with number | `88 marks` | Numeric value extracted |
| Invalid mark | `105` | Identified as invalid |

---

# 📂 Repository Structure

```text
pandas-Assignment/
│
├── README.md
│
└── pandas_Assignment/
    │
    ├── Parimalajyothika_Pandas.ipynb
    ├── student_assessment_dirty.csv
    └── students.csv
```

---

## 📓 Main Notebook

### `Parimalajyothika_Pandas.ipynb`

The main notebook contains:

- Assignment questions
- Python code
- Pandas operations
- NumPy operations
- Executed outputs
- Data analysis
- Data-cleaning operations
- Explanations of results

---

## 📄 Dataset Files

### `students.csv`

This dataset is used for CSV-based analysis and practical Pandas tasks.

### `student_assessment_dirty.csv`

This dataset is used for the Section D data-cleaning tasks.

It contains intentionally inconsistent and invalid values to demonstrate practical data-cleaning techniques.

---

# ▶️ How to Run the Project

## 🔹 Method 1 – Using Jupyter Notebook

### 1. Install Python

Download and install Python on your system.

Verify the installation using:

```bash
python --version
```

---

### 2. Install Required Libraries

Open Command Prompt or Terminal and run:

```bash
pip install pandas numpy jupyter
```

---

### 3. Clone the Repository

Clone the repository using Git:

```bash
git clone https://github.com/Ch-parimalajyothika/pandas-Assignment.git
```

---

### 4. Open the Project Folder

Move into the repository:

```bash
cd pandas-Assignment
```

Then move into the assignment folder:

```bash
cd pandas_Assignment
```

---

### 5. Start Jupyter Notebook

Run:

```bash
jupyter notebook
```

Jupyter Notebook will open in your default web browser.

---

### 6. Open the Notebook

Open:

```text
Parimalajyothika_Pandas.ipynb
```

---

### 7. Run the Notebook

Run the cells from top to bottom.

Alternatively, use:

```text
Kernel → Restart Kernel and Run All Cells
```

This ensures that the notebook is executed in the correct order.

---

# 🔹 Method 2 – Using Visual Studio Code

The notebook can also be executed using **Visual Studio Code**.

### Steps

1. Install Python.
2. Install Visual Studio Code.
3. Install the **Jupyter** extension.
4. Clone or download this repository.
5. Open the repository in VS Code.
6. Open the `pandas_Assignment` folder.
7. Open:

```text
Parimalajyothika_Pandas.ipynb
```

8. Select a Python/Jupyter kernel.
9. Run the notebook cells sequentially.
10. Alternatively, use **Run All** to execute the complete notebook.

---

# 📦 Required Libraries

The notebook uses the following Python libraries:

```python
import pandas as pd
import numpy as np
```

Install the required packages using:

```bash
pip install pandas numpy
```

For running the notebook through Jupyter:

```bash
pip install jupyter
```

---

# 📄 Input Data

The assignment uses CSV datasets to demonstrate data loading, manipulation, analysis, and cleaning.

The datasets include examples involving:

- Student information
- Marks
- Departments
- Dates
- Salaries
- Missing values
- Duplicate records
- Invalid values

The Section D dataset contains intentionally inconsistent values for demonstrating data-cleaning techniques.

### Example Department Values

```text
IT
it
I.T.
Finance
finance
```

### Example Marks Values

```text
88 marks
Absent
NA
blank values
105
```

These values are processed according to their meaning and validity during the cleaning process.

---

# 📊 Expected Results

After executing the notebook, the following types of results can be observed:

- Pandas Series outputs
- DataFrame outputs
- Statistical calculations
- Correlation results
- Filtered datasets
- Missing-value summaries
- Duplicate-record analysis
- Cleaned DataFrames
- Invalid-value identification
- Data-validation results

The notebook contains the corresponding executed outputs for the completed tasks.

---

# 🎓 Learning Outcomes

After completing this assignment, the following practical skills are demonstrated:

- Creating and manipulating Pandas Series
- Creating and manipulating DataFrames
- Reading CSV files
- Selecting and filtering data
- Sorting data
- Handling missing data
- Performing statistical analysis
- Calculating correlations
- Converting data types
- Working with dates
- Detecting duplicate records
- Standardizing inconsistent data
- Validating numerical data
- Handling invalid values
- Performing practical data cleaning

These concepts provide a foundation for further learning in:

- **Data Science**
- **Artificial Intelligence**
- **Machine Learning**
- **Data Analytics**

---

# 💻 Example Pandas Workflow

A basic Pandas workflow demonstrated in the assignment is:

```python
import pandas as pd

df = pd.read_csv("data.csv")

print(df.head())
print(df.info())
print(df.isnull().sum())
```

The DataFrame can then be selected, filtered, analyzed, validated, and cleaned according to the requirements of the task.

---

# 🔍 Notebook Execution Guidelines

For the best results:

- Run the notebook cells in the given order.
- Do not skip cells that create or modify DataFrames.
- Make sure the required CSV files are available.
- Use the correct file paths when loading datasets.
- Restart the kernel if previous variables cause unexpected results.
- Use **Run All** after restarting the kernel when executing the complete notebook.
- Make sure outputs are generated after running the required cells.

---

# 🔄 Overall Data Analysis Flow

The complete assignment demonstrates the following general process:

```text
Load Data
    ↓
Understand Data
    ↓
Select & Filter
    ↓
Analyze Data
    ↓
Inspect Data Quality
    ↓
Clean Data
    ↓
Validate Data
    ↓
Generate Results
```

### Dedicated Data-Cleaning Flow

```text
Load Data
    ↓
Inspect Data
    ↓
Standardize Data
    ↓
Remove Duplicates
    ↓
Handle Missing Values
    ↓
Convert & Clean Values
    ↓
Validate Data
    ↓
Handle Invalid Values
    ↓
Generate Clean Data
```

---

# 🌟 Project Highlights

- Covers **four assignment sections: A, B, C, and D**
- Demonstrates fundamental Pandas concepts
- Includes practical CSV processing
- Performs statistical analysis
- Demonstrates correlation analysis
- Handles missing and inconsistent values
- Identifies duplicate records
- Demonstrates data validation
- Performs practical data cleaning
- Uses both **Pandas and NumPy**
- Includes executed notebook outputs and explanations

---

# 👩‍💻 Author

**Parimala Jyothika**

**B.Tech – Computer Science and Engineering**

---

# 📌 Academic Purpose

This repository was created as part of an **academic Pandas assignment** to demonstrate practical knowledge of:

- Data analysis
- Data manipulation
- Statistical operations
- CSV processing
- Missing-value handling
- Data validation
- Data cleaning

The project is intended for **academic and educational purposes**.

---

# 📜 License

This project is intended for **academic and educational purposes**.
