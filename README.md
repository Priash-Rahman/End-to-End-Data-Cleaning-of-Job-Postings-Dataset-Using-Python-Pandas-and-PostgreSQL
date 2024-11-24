# End-to-End Data Cleaning of Job Postings Dataset Using Python (Pandas) and PostgreSQL.



## Project Overview

In this project, the goal is to clean and prepare a real-world dataset of job postings for data analysts, ensuring it is ready for further analysis and reporting. The dataset contains 13 columns with over 2,000 rows, including details such as job titles, salary ranges, company information, and job characteristics.

The project demonstrates a dual-environment approach using both Python and PostgreSQL to showcase versatility and proficiency in data cleaning across different tools. The cleaned dataset will provide accurate, consistent, and structured information suitable for insights into the data analytics job market.

### Steps followed 

#### Python (Pandas) Approach:
- Loaded the dataset into a Pandas DataFrame..
- Split salary ranges into minimum and maximum values. 
- Removed company ratings appended to company names (e.g., "Company Name\n3.2").
- Replaced invalid or placeholder values like -1 or 0 with NULL
- Standardized text fields for uniformity (e.g., revenue ranges and company sizes)
- Converted the Founded column to NULL where the value was 0.
- Encoded the Easy Apply column as binary values (0 or 1).
- Generated a clean CSV or DataFrame for further analysis.



#### PostgreSQL Approach: Interface (DBeaver)
- Created a table job_postings to represent the raw dataset
- Imported the raw data into PostgreSQL using DBeaver
## Cleaning steps : 

#### Step 1 : Prepare the environment , delete unneseccary columns , make a clone of raw data to maintain data integrity(SQL)
 

![Prepare the envo](https://github.com/user-attachments/assets/4e4de2b8-813b-4ca4-bbd0-5e2094aab26f)


 #### Step 2: Segment job title column into 5 category & add the new column in table.
![Screenshot 2024-11-23 094933](https://github.com/user-attachments/assets/b45707f3-3090-4fd2-9488-c548999be826)
#### Step 3: Split location column into 2 part City & State & add to the table


![Screenshot 2024-11-23 095504](https://github.com/user-attachments/assets/71c9517f-c593-4e47-a5d2-c64fefb52a35)


#### Step 3: Fix inconsistencies in "Size" column.
![fixed size column](https://github.com/user-attachments/assets/dd7b16f6-75b7-4d57-848f-32f89b18280b)

#### Step 4: Split salary column into min & max convert them to numeric.
![Screenshot 2024-11-23 150553](https://github.com/user-attachments/assets/7786a0c8-d1dc-4225-ac11-aa35b1d7fb78)
#### Step 5: Replace -1 with 'Unknown' in Founded column
![Screenshot 2024-11-23 202108](https://github.com/user-attachments/assets/8e79e3d2-5099-4c6f-9083-bd58cc6a3789)
#### Step 6: Replace -1 with Unknown at 3 columns at same time.
![3 columns fixed](https://github.com/user-attachments/assets/a3ab12a9-8665-4fbb-99c0-65ad3cdc0432)
#### Step 7: Replace -1 with 'Unknown' in competitors column.
![fixed competitors column](https://github.com/user-attachments/assets/428cb69f-ed04-4fb4-b5d6-2ef8011cfb95)

#### Step 8: Split company name column and create a separate rating column  
![Screenshot 2024-11-24 205429](https://github.com/user-attachments/assets/b824a25e-48f5-490a-b654-ab24f1281cb3)

