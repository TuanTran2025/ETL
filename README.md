# ETL

## 1. Introduction
In company, Information related to demographics, education, experience are in hands from candidates signup and enrollment.
However, these data are comming from several deppartments as well as in different format types.
This project introduces the ETL process in step by step to collect all relatted data, fix the missing data and then combine them into a database which is ready for analysis purpose.

## 2. Data information
### 2.1. Source of data
- Enrollies' data: https://docs.google.com/spreadsheets/d/1VCkHwBjJGRJ21asd9pxW4_0z2PWuKhbLR3gUHm-p4GI/edit?usp=sharing
- Enrollies' education: https://assets.swisscoding.edu.vn/company_course/enrollies_education.xlsx
- Enrollies' working experience: https://assets.swisscoding.edu.vn/company_course/work_experience.csv
- Training hours: from the Database with credentials as following: \
       -- Database type: MySQL \
       - Host: 112.213.86.31 \
       Port: 3360 \
       Login: etl_practice \
       Password: 550814 \
       Database name: company_course \
       Table name: training_hours
- City development index: in a table from the website https://sca-programming-school.github.io/city_development_index/index.html
- Employment: in an employment table from the same MySQL Database as above.

2.2. Data description
- Enrollies' data: \
       As enrollies are submitting their request to join the course via Google Forms, it has been created the Google Sheet that stores data about enrolled students, containing the following columns: \
       enrollee_id: unique ID of an enrollee \
       full_name: full name of an enrollee \
       city: the name of an enrollie's city \
       gender: gender of an enrollee
  
- Enrollies' education: \
After enrollment everyone should fill the form about their education level. This form is being digitalized manually. Educational department stores it in the Excel format file which has a table contains the following columns: \
       enrollee_id: A unique identifier for each enrollee. This integer value uniquely distinguishes each participant in the dataset. \
       enrolled_university: Indicates the enrollee's university enrollment status. Possible values include no_enrollment, Part time course, and Full time course. \
       education_level: Represents the highest level of education attained by the enrollee. Examples include Graduate, Masters, etc. \
       major_discipline: Specifies the primary field of study for the enrollee. Examples include STEM, Business Degree, etc.

## A description of each step and decision (for example, why you chose to perform the data cleaning in the way you did)

## Instruction, how to schedule the script on any platform (you can choose which platform you will write the instruction for). Don't forget, that you have instruction in the last lecture's Colab file.
