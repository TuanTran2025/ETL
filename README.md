# ETL

## 1. Introduction
In company, Information related to demographics, education, experience are in hands from candidates signup and enrollment.
However, these data are comming from several deppartments as well as in different format types.
This project introduces the ETL process in step by step to collect all relatted data, fix the missing data and then combine them into a database which is ready for analysis purpose.

## 2. Data Source
- Enrollies' data: https://docs.google.com/spreadsheets/d/1VCkHwBjJGRJ21asd9pxW4_0z2PWuKhbLR3gUHm-p4GI/edit?usp=sharing
- Enrollies' education: https://assets.swisscoding.edu.vn/company_course/enrollies_education.xlsx
- Enrollies' working experience: https://assets.swisscoding.edu.vn/company_course/work_experience.csv
- Training hours: from the Database with credentials as following: \
       * Database type: MySQL \
       * Host: 112.213.86.31 \
       * Port: 3360 \
       * Login: etl_practice \
       * Password: 550814 \
       * Database name: company_course \
       * Table name: training_hours
- City development index: in a table from the website https://sca-programming-school.github.io/city_development_index/index.html
- Employment: in an employment table from the same MySQL Database as above. \
---------------------
Other sources: https://github.com/TuanTran2025/ETL

## 3. Descriptions of main steps
### 3.1. Extract data
Data will be extracted from different types of source, such as:
- Google sheet: Enrollies' data
- Excel format: Enrollies' education
- CSV format: Enrollies' working experience
- MySQL database: Training hours and Employment
- Table from Website: City development index

### 3.2. Tranform data
- Fix data types: Due to optimizing the memory and processing time, it is necessary to converting the data types of related columns into properly ones, for instance: \
      * String type for full_name and experience columns. \
      * Category type for columns of gender, city, enrolled_university, education_level, major_discipline, etc.
- Fill missing values: In simple way, all missing values will be filled with the most frequent one.

### 3.3. Load data
In finale, all cleaned data will be load into a single database file which is included all related tables and now ready for analysis purpose.

