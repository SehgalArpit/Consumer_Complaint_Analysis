# Consumer Complaints Data Analysis

This repository contains the analysis of consumer complaints data using Excel. The analysis involves data cleaning, combining datasets, working with dates, and generating reports and dashboards. The project aims to provide insights into customer complaints, the resolution process, and reporting at different levels (company, product, etc.).

## Project Overview

The data consists of consumer complaints along with their state codes, complaint issues, resolution times, and company details. The project focuses on:

- **Data Preparation**: Combining and cleaning datasets, extracting relevant information.
- **Data Analysis**: Identifying trends, counting missing data, and analyzing complaint resolution.
- **Reporting**: Creating summary reports at both company and issue levels.
- **Dashboard Creation**: Generating visual insights into the complaint data.
  
## Tasks Breakdown

### **Task 1: Data Preparation and Combining Datasets**
1. **Create Columns**:
    - Add `STATE` and `CODE` columns to the `State_Code_Name` worksheet.
    - Extract and transform data from a JSON format into tabular form using Excel functions like `VLOOKUP`.
2. **Data Mapping**:
    - Create a `State_Name` column in the `Consumer_Complaints` worksheet.
    - Map the `State_Code` to `State_Name` using data from the `State_Code_Name` worksheet.
3. **Count Missing Data**:
    - Calculate the number of records with missing state names (`#N/A` values).
4. **Create Summary Table**:
    - Create a summary table for complaints where the `State_Name` is not mapped.
5. **Inferences**:
    - Analyze potential reasons for missing state names in the data.

### **Task 2: Working with Dates**
1. **Calculate Resolution Time**:
    - Calculate the resolution time in days for complaints based on the complaint and resolution dates.
2. **Year and Quarter Columns**:
    - Add a `YEAR` column to extract the year from the complaint received date.
    - Add a `QTR` column to determine the fiscal quarter (Q1, Q2, Q3, Q4) based on the complaint date.
3. **Data Cleaning**:
    - Ensure all date columns are in the correct date format (mm/dd/yyyy or dd-mm-yyyy).

### **Task 3: Reporting at Company Level**
1. **Company-wise Complaints**:
    - Summarize the total number of complaints for each company.
2. **Timely Response**:
    - Calculate the number and percentage of complaints where no timely response was provided.
3. **Disputed Complaints**:
    - Calculate the number and percentage of disputed complaints.
4. **Average Delay**:
    - Calculate the average delay in days for complaints.

### **Task 4: Reporting and Visualization**
1. **Top 5 Companies with Complaints**:
    - Display the top five companies with the most complaints.
2. **Top 5 Issues with Complaints**:
    - Display the top five complaint issues based on the number of complaints.
3. **Monthly Trends**:
    - Create a line/area chart to visualize the monthly trend of complaints.

### **Task 5: Dashboard Creation**
1. **Key Performance Indicators (KPIs)**:
    - Display KPIs such as total complaints, timely responses, and average resolution time with YoY change.
2. **Proportions by Product and Channel**:
    - Display the proportion of complaints by product type and the channel used for filing the complaints.
3. **Priority Complaints**:
    - Graphically display which complaints should be prioritized based on urgency.
4. **Monthly Trends**:
    - Create a line or area chart to show the monthly trend of complaints over time.

## How to Use

1. **Clone the Repository**:
    - To get started, clone the repository using the following command:
    ```bash
    git clone https://github.com/your-username/consumer-complaints-analysis.git
    ```

2. **Data Files**:
    - All data for analysis is stored in the `Consumer_Complaints` and `State_Code_Name` worksheets. Ensure the data is correctly formatted before running the analysis.

3. **Analysis Steps**:
    - Follow the task breakdown above to perform the data preparation, analysis, and reporting steps using Excel. Use features like **Pivot Tables**, **VLOOKUP**, **COUNTIF**, **Charts**, and **IFS** to process the data.

4. **Report Creation**:
    - After completing the analysis, use Excel to create reports for each task (company-wise summaries, issue-wise complaints, etc.). Add charts and summaries as needed.

5. **Dashboard**:
    - Create a new worksheet called `Report_Task5` to build the dashboard and display the KPIs and trends.

## Tools Used
- **Excel**: For data cleaning, analysis, pivot tables, charts, and dashboards.
- **Formulas**: `VLOOKUP`, `COUNTIF`, `DATEDIF`, `YEAR`, `MONTH`, etc., for data calculations and mapping.

## Inferences

- The analysis helps identify trends and key performance indicators such as the average resolution time and timely responses for each company.
- Insights from the analysis can guide customer support teams in prioritizing complaints and improving response times.
- The dashboard provides a comprehensive view of complaint trends, product performance, and response metrics.

## Acknowledgements

- The data for this project was sourced from publicly available datasets.
- Thank you to those who contributed to the open-source tools used for data cleaning and analysis.
