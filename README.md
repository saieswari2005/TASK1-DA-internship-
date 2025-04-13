# TASK1-DA-internship
this is about my data analyst internship of task 1
Task 1: Data Cleaning and Preprocessing – Customer Shopping Data
✅ Objective
To clean and preprocess a raw dataset containing missing values, duplicates, inconsistent formats, and improper column names using Python (Pandas).

📁 Dataset Used
customer_shopping_data.csv
Sample columns include: Invoice ID, Gender, Age, Category, Quantity, Price, Date

🛠️ Steps Performed
Data Loading

Loaded the CSV file using pandas.read_csv().

Handling Missing Values

Used ffill() to forward-fill missing values where possible.

Removing Duplicate Rows

Identified and removed duplicate rows using drop_duplicates().

Standardizing Text Data

Converted values in Gender and Category columns to lowercase and removed extra spaces.

Date Format Conversion

Checked for any column with "date" in its name and converted it to datetime format.

Column Renaming

Standardized column headers to lowercase and replaced spaces with underscores using:

python
Copy
Edit
df.columns.str.lower().str.replace(' ', '_')
Data Type Fixes

Converted Age, Quantity, and Price to integers for consistency.

Saved the Cleaned Dataset

Exported the cleaned DataFrame to cleaned_customer_shopping_data.csv.
