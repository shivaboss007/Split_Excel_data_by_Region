# Split_Excel_data_by_Region

Split Excel Data by Region using Python
📌 Overview

This project automates the process of splitting a large Excel dataset into multiple files based on regions using Python.

It is useful for businesses and analysts who need to organize, distribute, or analyze region-wise data efficiently.

🎯 Objective
Read a large Excel dataset
Group data based on a region column
Automatically create separate Excel files for each region
Improve data organization and usability
🛠️ Tech Stack
Python
Pandas
OpenPyXL / XlsxWriter
Jupyter Notebook

⚙️ How It Works
Load the Excel file using Pandas
Identify the region column
Group the dataset using groupby()
Loop through each region
Export each group as a separate Excel file


Sample Code
import pandas as pd

# Load dataset
df = pd.read_excel("input_data.xlsx")

# Group by region and save files
for region, data in df.groupby("Region"):
    file_name = f"{region}.xlsx"
    data.to_excel(file_name, index=False)

# How to Run
Clone the repository:
git clone https://github.com/shivaboss007/Split_Excel_data_by_Region.git
Navigate to the folder:
cd split_excel_data_by_region
Install dependencies:
pip install pandas openpyxl
Run the notebook:
jupyter notebook

# Use Cases
Sales data distribution by region
Branch-wise reporting
Data cleaning & preprocessing
Business intelligence workflows

# Contact: 
https://www.linkedin.com/in/shivkumar-tummaghunta/

# Open to opportunities in:

Data Analytics
Data-driven QA
Automation & Reporting
