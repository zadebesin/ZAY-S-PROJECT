Employee Salary Data Processing Project

This project demonstrates how to:

Import employee data from a CSV file.
Define a function to retrieve employee details based on their name.
Process the data into a dictionary format.
Implement error handling to manage potential issues.
Export employee data to a CSV file, and zip it into a folder.
Use R to unzip the folder and display the data.
This project consists of a Python script and an R script to work with employee salary and personal data.

Installation
1. Requirements

Python:
pandas library for data manipulation.
zipfile for compressing files.
Install panda

R:
readr (or just base R) for reading CSV files.
2. Files Included
salary_data.csv — A sample CSV file containing employee data.
Salary data.py — Python script for processing employee data.
salary data.R — R script for unzipping and displaying employee data.
README.md — Documentation for this project.

Project Description
Python Script: employee_processing.py
The Python script performs the following tasks:

1. Import Data
The script starts by importing employee data from a CSV file (employee_data.csv) using the pandas library. The data is loaded into a pandas DataFrame, making it easy to process.
2. Create Employee Function
A function get_employee_details(name) is defined to accept an employee's name as input and return their details. It checks if the employee exists and returns the corresponding data or an error message if not found.
3. Data Processing with Dictionary
The employee data is converted into a dictionary format, where the employee name is the key, and the value is a dictionary containing their job title, basepay, otherpay and totalpay.
4. Export Employee Details to CSV and Zip
A function export_to_csv_and_zip(name) is used to export employee data to a CSV file. The CSV file is then compressed into a ZIP file to save it as an archive.

R Script: salary data.R
The R script handles unzipping the folder, reading the extracted CSV file, and displaying the data.

1. Unzip the Folder
The ZIP file is unzipped into a folder named Employee_Profile.
2. List Files in the Folder
The script lists the files in the folder to verify that the CSV file has been extracted correctly.
3. Read and Display the Data

How to Run
1. Python Code
To run the Python script:

Ensure you have Python installed along with the required libraries (pandas).
Place the salary_data.csv file in the same directory as the Python script.
Run the Python script from the terminal or command prompt:
This will load the employee data, process it, and export the details for a specific employee to a CSV file, which is then zipped into a folder.

2. R Code
To run the R script:

Ensure you have R installed on your system.
Place the ZIP file (Employee_Profile.zip) in the same directory as the R script.
Open an R console or RStudio, and run the following command:
This will unzip the file and display the employee details in the R console.

Expected Output
1. Python Output
After running the Python script, the console will show the success or error messages, and a ZIP file Employee_Profile.zip will be created in the working directory. The ZIP file contains a CSV with the employee details.

2. R Output
After running the R script, the employee data will be displayed in the R console