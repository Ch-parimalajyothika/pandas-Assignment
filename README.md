# 📊 Pandas Assignment – Data Analysis & Data Cleaning

## 📌 Overview

This repository contains my **Pandas Assignment**, implemented using **Python, Pandas, and NumPy** in a Jupyter Notebook.

The assignment demonstrates fundamental and practical concepts of Pandas, including **Series and DataFrames, data manipulation, statistical analysis, correlation analysis, CSV processing, missing-value handling, and real-world data cleaning**.

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
- Detect and handle invalid values
- Perform practical data-cleaning operations

---

## 🛠️ Technologies Used

- **Python**
- **Pandas**
- **NumPy**
- **Jupyter Notebook**
- **Visual Studio Code** (optional)

---

## 📚 Assignment Contents

The assignment is divided into **four sections: A, B, C, and D**.

### 🔹 Section A – Pandas Fundamentals

This section covers the basic concepts and operations of Pandas:

- Pandas Series
- Pandas DataFrames
- Creating and accessing DataFrames
- Data selection
- Statistical operations
- Grouping and analysis
- Correlation analysis

### 🔹 Section B – Pandas Operations

This section focuses on commonly used Pandas operations:

- Reading CSV files
- Sorting data
- Handling missing values
- Working with DataFrame columns
- Calculating correlation between columns

### 🔹 Section C – Practical Data Analysis

This section demonstrates practical data-analysis techniques:

- Broadcasting
- CSV data processing
- Missing-value inspection
- Date conversion
- Data type handling
- Mean and median calculation
- Handling extreme values
- Identifying maximum values

### 🔹 Section D – Data Cleaning

This section focuses on real-world data-cleaning tasks:

- Inspecting dataset structure using `head()`, `info()`, and `isnull().sum()`
- Standardizing inconsistent department names
- Removing exact duplicate records
- Handling `"Absent"`, `"NA"`, and blank values
- Distinguishing between **Absent** and **Not Entered**
- Extracting numeric values from entries such as `"88 marks"`
- Identifying values outside the valid `0–100` range
- Handling invalid marks
- Reporting removed records and remaining missing values
- Displaying the final cleaned DataFrame

---

## 📂 Repository Structure

```text
Pandas-Assignment/
│
├── Parimalajyothika_Pandas.ipynb
└── README.md
```

### 📓 Main Notebook

**`Parimalajyothika_Pandas.ipynb`**

The notebook contains the complete assignment with:

- Questions
- Python/Pandas code
- Executed outputs
- Data analysis
- Data-cleaning operations
- Explanations for the results

---

# ▶️ How to Run the Project

## 🔹 Method 1 – Using Jupyter Notebook

### 1. Install Python

Download and install **Python** on your system.

You can verify the installation using:

```bash
python --version
```

### 2. Install the Required Libraries

Open **Command Prompt** or **Terminal** and run:

```bash
pip install pandas numpy jupyter
```

This installs the main libraries required to execute the notebook.

### 3. Clone the Repository

Clone this repository using Git:

```bash
git clone <repository-url>
```

> Replace `<repository-url>` with the actual GitHub repository URL.

### 4. Open the Project Folder

Move into the cloned repository folder:

```bash
cd Pandas-Assignment
```

### 5. Start Jupyter Notebook

Run:

```bash
jupyter notebook
```

Jupyter Notebook will open in your default web browser.

### 6. Open the Notebook

From the Jupyter Notebook interface, open:

```text
Parimalajyothika_Pandas.ipynb
```

### 7. Run the Notebook

Run the cells **from top to bottom**.

Alternatively, use:

**Kernel → Restart Kernel and Run All Cells**

This ensures that all cells are executed in the correct order and that the required outputs are generated.

---

# 🔹 Method 2 – Using VS Code

The notebook can also be executed using **Visual Studio Code**.

### Steps

1. Install **Python**.
2. Install **Visual Studio Code**.
3. Open VS Code.
4. Install the **Jupyter** extension.
5. Clone or download this repository.
6. Open the repository folder in VS Code.
7. Open:

```text
Parimalajyothika_Pandas.ipynb
```

8. Select a Python/Jupyter kernel.
9. Run the notebook cells sequentially.
10. Alternatively, select **Run All** to execute all cells.

---

## 📦 Required Libraries

The notebook uses the following Python libraries:

```python
import pandas as pd
import numpy as np
```

Install them using:

```bash
pip install pandas numpy
```

For running the notebook through Jupyter, install:

```bash
pip install jupyter
```

---

# 📄 Input Data

The notebook uses CSV datasets to demonstrate data loading, analysis, manipulation, and cleaning operations.

The datasets include examples involving:

- Student information
- Marks
- Departments
- Dates
- Salaries
- Missing values
- Duplicate records
- Invalid values

The data-cleaning section contains intentionally inconsistent values to demonstrate practical data-cleaning techniques.

### Examples of inconsistent department values

```text
IT
it
I.T.
```

These values are standardized into a consistent department format.

### Examples of marks-related values

```text
88 marks
Absent
NA
blank values
105
```

These values are processed according to their meaning and validity during the data-cleaning process.

---

# 🧹 Data Cleaning Process

The notebook demonstrates a practical data-cleaning workflow.

## 1. Data Inspection

The dataset is first inspected using:

```python
df.head()
df.info()
df.isnull().sum()
```

These operations help understand the dataset structure, data types, and missing values.

---

## 2. Standardization

Inconsistent department names are standardized into consistent categories.

For example:

```text
IT
it
I.T.
```

are standardized as:

```text
IT
```

This ensures consistent categorical values during analysis.

---

## 3. Duplicate Removal

Exact duplicate records are identified and removed.

This prevents duplicate information from affecting statistical analysis and the final dataset.

---

## 4. Missing-Value Handling

Different types of missing information are considered separately:

- `Absent`
- `NA`
- Blank values
- `Not Entered`

The assignment distinguishes between **Absent** and **Not Entered** instead of automatically treating all missing information in the same way.

This helps preserve meaningful information during data cleaning.

---

## 5. Numeric Conversion

Values containing text along with numbers are processed appropriately.

For example:

```text
88 marks
```

is converted into:

```text
88
```

This allows the value to be used for numerical analysis.

---

## 6. Invalid-Value Detection

Marks are checked against the valid range:

```text
0 – 100
```

Values outside this range are identified as invalid and handled appropriately.

For example:

```text
105
```

is identified as an invalid mark because it is outside the valid range.

---

# 📊 Expected Results

After executing the notebook, users can observe:

- Series and DataFrame outputs
- Statistical calculations
- Correlation results
- Filtered datasets
- Missing-value summaries
- Duplicate-record analysis
- Cleaned DataFrames
- Invalid-value identification
- Data-validation results

The notebook contains the executed outputs and explanations for the completed assignment.

---

# 🎓 Learning Outcomes

After completing this assignment, the following practical skills are demonstrated:

- Creating and manipulating Pandas DataFrames
- Working with Pandas Series
- Reading CSV files
- Selecting and filtering data
- Performing statistical analysis
- Calculating correlations
- Handling missing data
- Converting data types
- Detecting duplicate records
- Standardizing inconsistent data
- Validating data
- Cleaning real-world datasets

These skills provide a foundation for further work in:

- **Data Science**
- **Artificial Intelligence**
- **Machine Learning**
- **Data Analytics**

---

# 💻 Example Pandas Workflow

A typical workflow demonstrated in this assignment is:

```python
import pandas as pd

df = pd.read_csv("data.csv")

print(df.head())
print(df.info())
print(df.isnull().sum())
```

The dataset can then be processed, analyzed, validated, and cleaned according to the requirements of each task.

---

# 📁 File Information

| File | Description |
|------|-------------|
| `Parimalajyothika_Pandas.ipynb` | Complete Pandas assignment notebook |
| `README.md` | Project documentation |

---

# 🚀 How to Use This Repository

Follow these steps to use the project:

1. **Clone or download** the repository.
2. **Install Python** if it is not already installed.
3. **Install the required libraries** using `pip`.
4. Open `Parimalajyothika_Pandas.ipynb`.
5. Select a **Python/Jupyter kernel**.
6. Make sure the required CSV files are available in the expected location.
7. Run the notebook cells **from top to bottom**.
8. Review the generated outputs and explanations.

The notebook is designed to be **self-contained and easy to follow** for users familiar with basic Python.

---

# 🔍 Notebook Execution Guidelines

For the best results:

- Run the cells in the given order.
- Do not skip cells that create or modify DataFrames.
- Make sure required CSV files are available before execution.
- Restart the kernel if previous variables or outputs cause unexpected results.
- Use **Run All** after restarting the kernel when you want to execute the complete notebook from the beginning.

---

# 📌 Project Highlights

This assignment demonstrates the complete flow of basic data analysis:

```text
Load Data
    ↓
Inspect Data
    ↓
Select & Filter
    ↓
Analyze Data
    ↓
Handle Missing Values
    ↓
Standardize Data
    ↓
Remove Duplicates
    ↓
Validate Data
    ↓
Handle Invalid Values
    ↓
Generate Clean Data
```

---

# 👩‍💻 Author

**Parimala Jyothika**

**B.Tech – Computer Science and Engineering**

---

# 📌 Academic Purpose

This repository is created as part of an **academic Pandas assignment** to demonstrate practical knowledge of data analysis, data manipulation, statistical operations, and data-cleaning techniques using Python.

---

# 📜 License

This project is intended for **academic and educational purposes**.
