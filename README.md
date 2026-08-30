# AI Data Analyzer & Cleaning Tool

A Python-based command-line tool for analyzing and cleaning CSV datasets.

## 📌 About

**AI Data Analyzer & Cleaning Tool** is a Python project designed to make basic dataset analysis and cleaning easier through an interactive command-line interface.

The program allows users to load a CSV dataset, view important dataset information, clean missing values, remove duplicate rows, generate missing-value summaries, and save cleaned data.

## ✨ Features

- 📂 Load CSV datasets
- 📊 View basic dataset information
  - First 5 records
  - Number of rows
  - Number of columns
  - Column names
  - Missing values
  - Duplicate rows
- 🧹 Handle missing values
  - Manual value
  - Mean
  - Median
  - Minimum
  - Mode
  - Drop rows
  - `"Unknown"` value
- ♻️ Remove duplicate rows
- 📈 Generate missing-value summaries
- 💾 Save cleaned datasets as CSV
- 🗄️ Save cleaned data to MySQL
- 📝 Save and view cleaning history reports in JSON
- 🔄 Interactive menu-based interface

## 🛠️ Technologies Used

- Python
- Pandas
- MySQL
- SQLAlchemy
- JSON

## 📋 Main Menu

The program provides the following options:

```text
1. Load Dataset
2. Basic Info
3. Data Cleaning
4. Quit
```

### Data Cleaning Menu

```text
1. Null Handling
2. Handle Duplicates
3. Save Cleaned Dataset
4. Missing Value Summary
5. View Cleaning History
6. Back
```

## 🧹 Missing Value Handling

For numerical columns, the program supports:

```text
1. Enter value manually
2. Fill with Average
3. Fill with Median
4. Fill with Minimum
```

For object/string columns:

```text
1. Enter value manually
2. Fill with Mode
3. Drop rows containing missing values
4. Fill with "Unknown"
```

## 💾 Export Options

After cleaning a dataset, the program can save the result as:

### CSV

The user enters a filename and the cleaned dataset is saved with the `.csv` extension.

### MySQL

The program can connect to MySQL and save the cleaned dataset into the `cleaned_data` table.

## 📊 Cleaning History

The program records dataset information before and after cleaning, including:

- Number of rows
- Missing values
- Number of duplicate rows

The report can be saved as:

```text
report.json
```

## 🚀 How to Run

Install the required Python libraries:

```bash
pip install pandas mysql-connector-python sqlalchemy
```

Then run:

```bash
python your_file_name.py
```

Enter the path of your CSV dataset when prompted.

## 📁 Project Workflow

```text
Load Dataset
     ↓
View Basic Information
     ↓
Clean Dataset
     ├── Handle Missing Values
     ├── Remove Duplicates
     └── Generate Missing Value Summary
     ↓
Save Cleaned Dataset
     ├── CSV
     └── MySQL
     ↓
Save Cleaning History
```

## 🎯 Project Goal

The goal of this project is to build practical experience with **Python, Pandas, data cleaning, database connectivity, and data-processing workflows**.

## 👨‍💻 Author

Faraz

Built as a Python data-handling and cleaning project.