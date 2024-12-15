# data-analyst-zaryab

Exploratory Data Analysis

Project Description:

Developed an exploratory analysis pipeline to evaluate the operational health of project management businesses in Downtown Vancouver using historical business licence data from 2013 to 2024.

Project Title:

"Operational Health Assessment of Project Management Businesses in Downtown Vancouver"

Objective:

To analyze the count and percentage distribution of business licence statuses (Active, Expired, Suspended, etc.) and derive actionable insights for policy decisions and resource allocation.

Dataset:

Source: City of Vancouver Open Data Portal

Name: Business Licences 2013 to 2024

Records: Filtered 781,013 records to under 500 by focusing on Downtown Vancouver and project management business subtype.

Methodology:

Data Cleaning and Profiling:

Removed duplicates, handled missing values, and standardized formats using AWS Glue DataBrew.

Mapped licence statuses to numeric categories for further analysis.

Data Processing and Metric Calculation:

Applied AWS Glue ETL to group licences by status and compute their distribution.

Created a dummy column for seamless data merging and utilized SQL queries for data extraction.

Visualization:

Grouped and calculated percentages to visualize operational health trends.

Tools and Technologies:

Data Storage: AWS S3

Data Processing: AWS Glue, AWS Glue DataBrew

Analysis: SQL, AWS Athena

Monitoring: AWS CloudWatch

Deliverables:

Count and percentage distribution of business licence statuses.

Grouped datasets stored in S3 for further use.

Insights on operational health trends of project management businesses.




Descriptive Analysis

Project Description:

Designed and implemented a descriptive analysis pipeline to calculate the average lifespan of business licences for project management businesses in Downtown Vancouver from 2013 to 2024.

Project Title:

"Average Lifespan Analysis of Project Management Business Licences in Downtown Vancouver"

Objective:

To compute and analyze the yearly average number of days between issue and expiry dates of business licences to support city planning and business continuity strategies.

Dataset:

Source: City of Vancouver Open Data Portal

Name: Business Licences 2013 to 2024

Records: Filtered 781,013 records to under 500 by focusing on Downtown Vancouver and project management business subtype.

Methodology:

Data Cleaning and Profiling:

Standardized column names and removed irrelevant fields using AWS Glue DataBrew.

Addressed missing expiry dates by imputing logical substitutes (e.g., current date for active licences).

Metric Calculation:

Used AWS Glue ETL to compute the difference between issue and expiry dates.

Applied SQL queries to calculate the average lifespan metric.

Storage:

Saved processed data in S3 buckets in CSV and Parquet formats for cost-effective access and scalability.

Tools and Technologies:

Data Storage: AWS S3

Data Processing: AWS Glue, AWS Glue DataBrew

Analysis: SQL, AWS Athena

Deliverables:

Calculated average licence lifespan by year (2013 to 2024).

Processed datasets stored in S3 for visualization and policy formulation.

Key insights into business continuity trends to inform strategic planning.
