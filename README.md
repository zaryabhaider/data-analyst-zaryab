<h1>Project 1: Exploratory Data Analysis</h1>

<h2>
    Project Description:
</h2>
Developed an exploratory analysis pipeline to evaluate the operational health of project management businesses in Downtown Vancouver using historical business licence data from 2013 to 2024.

<h2>
    Project Title:
</h2>
"Operational Health Assessment of Project Management Businesses in Downtown Vancouver"

<h2>
    Objective:
</h2>
To analyze the count and percentage distribution of business licence statuses (Active, Expired, Suspended, etc.) and derive actionable insights for policy decisions and resource allocation.

<h2>
    Dataset Source:
</h2>
<a href="https://opendata.vancouver.ca/pages/home/">
    City of Vancouver Open Data Portal
</a>

<h2>
    Name:
</h2>
<a href="https://opendata.vancouver.ca/explore/dataset/business-licences-2013-to-2024/information/?disjunctive.status&localarea=Downtown&refine.city=Vancouver&q=project&refine.localarea=Downtown&refine.businesssubtype=Project+Management">
    Business Licences 2013 to 2024
</a>

<h2>
    Records:
</h2>
Filtered 781,013 records to under 500 by focusing on Downtown Vancouver and project management business subtype.

<h2>
    Methodology:
</h2>

<li>
    Data Cleaning and Profiling: Removed duplicates, handled missing values, and standardized formats using AWS Glue DataBrew.
</li>
<li>
    Mapped licence statuses to numeric categories for further analysis.
</li>
<li>
    Data Processing and Metric Calculation:
</li>
<li>
    Applied AWS Glue ETL to group licences by status and compute their distribution.
</li>
<li>
    Created a dummy column for seamless data merging and utilized SQL queries for data extraction.
</li>

<h2>
    Visualization:
</h2>
![Picture1](https://github.com/user-attachments/assets/007773b8-4fea-4047-b049-37aaca46877c)


Grouped and calculated percentages to visualize operational health trends.

<h2>
    Tools and Technologies:
</h2>
<li>
    Data Storage: AWS S3
</li>
<li>
    Data Processing: AWS Glue, AWS Glue DataBrew
</li>
<li>
    Analysis: SQL, AWS Athena
</li>
<li>
    Monitoring: AWS CloudWatch
</li>

<h2>
    Deliverables:
</h2>
<li>
    Count and percentage distribution of business licence statuses.
</li>
<li>
    Grouped datasets stored in S3 for further use.
</li>
<li>
    Insights on operational health trends of project management businesses.
</li>


<br/>
<br/>



<h1>Project 2: Descriptive Analysis</h1>

<h2>
    Project Description:
</h2>
Designed and implemented a descriptive analysis pipeline to calculate the average lifespan of business licences for project management businesses in Downtown Vancouver from 2013 to 2024.

<h2>
    Project Title:
</h2>
"Average Lifespan Analysis of Project Management Business Licences in Downtown Vancouver"

<h2>
    Objective:
</h2>
To compute and analyze the yearly average number of days between issue and expiry dates of business licences to support city planning and business continuity strategies.

<h2>
    Dataset Source:
</h2>
<a href="https://opendata.vancouver.ca/pages/home/">
    City of Vancouver Open Data Portal
</a>

<h2>
    Name:
</h2>
<a href="https://opendata.vancouver.ca/explore/dataset/business-licences-2013-to-2024/information/?disjunctive.status&localarea=Downtown&refine.city=Vancouver&q=project&refine.localarea=Downtown&refine.businesssubtype=Project+Management">
    Business Licences 2013 to 2024
</a>

<h2>
    Records:
</h2>
Filtered 781,013 records to under 500 by focusing on Downtown Vancouver and project management business subtype.

<h2>
    Methodology:
</h2>
<li>
    Data Cleaning and Profiling:
</li>
<li>
    Standardized column names and removed irrelevant fields using AWS Glue DataBrew.
</li>
<li>
    Addressed missing expiry dates by imputing logical substitutes (e.g., current date for active licences).
</li>
<li>
    Metric Calculation:
</li>

<li>
    Used AWS Glue ETL to compute the difference between issue and expiry dates.
</li>
<li>
    Applied SQL queries to calculate the average lifespan metric.
</li>

<h2>
    Storage:
</h2>
Saved processed data in S3 buckets in CSV and Parquet formats for cost-effective access and scalability.

<h2>
    Tools and Technologies:
</h2>
<li>
    Data Storage: AWS S3
</li>
<li>
    Data Processing: AWS Glue, AWS Glue DataBrew
</li>
<li>
    Analysis: SQL, AWS Athena
</li>

<h2>
    Deliverables:
</h2>

<li>
    Calculated average licence lifespan by year (2013 to 2024).
</li>
<li>
    Processed datasets stored in S3 for visualization and policy formulation.
</li>
<li>
    Key insights into business continuity trends to inform strategic planning.
</li>
