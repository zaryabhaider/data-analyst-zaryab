# data-analyst-zaryab

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portfolio Page</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            line-height: 1.6;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
            color: #333;
        }
        header {
            background: #4CAF50;
            color: white;
            padding: 10px 20px;
            text-align: center;
        }
        section {
            margin: 20px;
            padding: 20px;
            background: white;
            border-radius: 5px;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }
        h2 {
            color: #4CAF50;
            border-bottom: 2px solid #4CAF50;
            padding-bottom: 5px;
        }
        ul {
            list-style: none;
            padding: 0;
        }
        ul li {
            background: #f1f1f1;
            margin: 5px 0;
            padding: 10px;
            border-left: 4px solid #4CAF50;
        }
        .section-title {
            margin-top: 0;
        }
    </style>
</head>
<body>

<header>
    <h1>Project Portfolio</h1>
</header>

<section>
    <h2>1) Exploratory Data Analysis</h2>

    <h3 class="section-title">Project Description:</h3>
    <p>Developed an exploratory analysis pipeline to evaluate the operational health of project management businesses in Downtown Vancouver using historical business licence data from 2013 to 2024.</p>

    <h3>Project Title:</h3>
    <p>"Operational Health Assessment of Project Management Businesses in Downtown Vancouver"</p>

    <h3>Objective:</h3>
    <p>To analyze the count and percentage distribution of business licence statuses (Active, Expired, Suspended, etc.) and derive actionable insights for policy decisions and resource allocation.</p>

    <h3>Dataset:</h3>
    <ul>
        <li>Source: City of Vancouver Open Data Portal</li>
        <li>Name: Business Licences 2013 to 2024</li>
        <li>Records: Filtered 781,013 records to under 500 by focusing on Downtown Vancouver and project management business subtype.</li>
    </ul>

    <h3>Methodology:</h3>
    <ol>
        <li><strong>Data Cleaning and Profiling:</strong> Removed duplicates, handled missing values, and standardized formats using AWS Glue DataBrew.</li>
        <li><strong>Data Processing and Metric Calculation:</strong> Applied AWS Glue ETL to group licences by status and compute their distribution.</li>
        <li><strong>Visualization:</strong> Grouped and calculated percentages to visualize operational health trends.</li>
    </ol>

    <h3>Tools and Technologies:</h3>
    <ul>
        <li><strong>Data Storage:</strong> AWS S3</li>
        <li><strong>Data Processing:</strong> AWS Glue, AWS Glue DataBrew</li>
        <li><strong>Analysis:</strong> SQL, AWS Athena</li>
        <li><strong>Monitoring:</strong> AWS CloudWatch</li>
    </ul>

    <h3>Deliverables:</h3>
    <ul>
        <li>Count and percentage distribution of business licence statuses.</li>
        <li>Grouped datasets stored in S3 for further use.</li>
        <li>Insights on operational health trends of project management businesses.</li>
    </ul>
</section>

<section>
    <h2>2) Descriptive Analysis</h2>

    <h3 class="section-title">Project Description:</h3>
    <p>Designed and implemented a descriptive analysis pipeline to calculate the average lifespan of business licences for project management businesses in Downtown Vancouver from 2013 to 2024.</p>

    <h3>Project Title:</h3>
    <p>"Average Lifespan Analysis of Project Management Business Licences in Downtown Vancouver"</p>

    <h3>Objective:</h3>
    <p>To compute and analyze the yearly average number of days between issue and expiry dates of business licences to support city planning and business continuity strategies.</p>

    <h3>Dataset:</h3>
    <ul>
        <li>Source: City of Vancouver Open Data Portal</li>
        <li>Name: Business Licences 2013 to 2024</li>
        <li>Records: Filtered 781,013 records to under 500 by focusing on Downtown Vancouver and project management business subtype.</li>
    </ul>

    <h3>Methodology:</h3>
    <ol>
        <li><strong>Data Cleaning and Profiling:</strong> Standardized column names and removed irrelevant fields using AWS Glue DataBrew.</li>
        <li><strong>Metric Calculation:</strong> Used AWS Glue ETL to compute the difference between issue and expiry dates.</li>
        <li><strong>Storage:</strong> Saved processed data in S3 buckets in CSV and Parquet formats for cost-effective access and scalability.</li>
    </ol>

    <h3>Tools and Technologies:</h3>
    <ul>
        <li><strong>Data Storage:</strong> AWS S3</li>
        <li><strong>Data Processing:</strong> AWS Glue, AWS Glue DataBrew</li>
        <li><strong>Analysis:</strong> SQL, AWS Athena</li>
    </ul>

    <h3>Deliverables:</h3>
    <ul>
        <li>Calculated average licence lifespan by year (2013 to 2024).</li>
        <li>Processed datasets stored in S3 for visualization and policy formulation.</li>
        <li>Key insights into business continuity trends to inform strategic planning.</li>
    </ul>
</section>

</body>
</html>

