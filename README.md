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

#### Step 1 : Prepare the environment , delete unneseccary columns , make a clone of raw data to maintain data integrity
 

 ![Prepare the envo](https://github.com/user-attachments/assets/2d701e05-0087-4d94-94db-1e60844e2eaa)

 ### Step 2: Segment job title column into 5 category & add the new column in table.
![Setmented job title](https://github.com/user-attachments/assets/eb154595-da9d-427b-80fe-0874098146f1)
#### Step 3: Split location column into 2 part City & State & add to the table

![Splitted city and state](https://github.com/user-attachments/assets/9585c253-f6b9-4aa1-a456-60633ada86a8)
