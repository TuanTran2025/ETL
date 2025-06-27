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
- Employment: in an employment table from the same MySQL Database as above.

## A description of each step and decision (for example, why you chose to perform the data cleaning in the way you did)
## 3. Descriptions of main steps
### 3.1. Extract data
Data will be extracted rom different types of source, such as:
- Google sheet: Enrollies' data
- Excel format: Enrollies' education
- CSV format: Enrollies' working experience
- MySQL database: Training hours and Employment
- Table from Website: City development index

### 3.2. Clean data
- Fix data types: Converting the data types of related columns into properly ones, for examples: \
      * Category type for columns of gender, city, enrolled_university, education_level, major_discipline, company_type, company_size and relevent_experience. \
      * String type for full_name and experience columns.
- Fill missing values:

## Instruction, how to schedule the script on any platform (you can choose which platform you will write the instruction for). Don't forget, that you have instruction in the last lecture's Colab file.
