# Power-BI-Project
Power BI Data Survey Project
<title>Data Professionals Power BI Dashboard</title>
</head>
<body>

    <h1>Data Professionals Power BI Dashboard</h1>

    <h2>Description</h2>
    <p>
        The <strong>Data Professionals Power BI Dashboard</strong> project focuses on visualizing insights from a dataset of individuals in various data-related roles. 
        The project began by preparing and transforming the raw survey data to ensure only relevant information was included. 
        Unnecessary columns and rows were removed using Power BI’s <strong>Remove Columns</strong> and <strong>Split Column</strong> features, with further refinement 
        through custom filtering to exclude inconsistent or irrelevant user inputs.
    </p>
    <p>
        One of the primary tasks involved cleaning the salary data. Originally formatted as a range (e.g., “50k-60k”), this was split into two separate columns using 
        <strong>Split Column by Delimiter</strong>, and then recombined in a custom column to calculate the average salary using the following formula:
    </p>
    <pre>
= Table.AddColumn(#"Removed Columns7", "Average", each ([#"Q3 - Current Yearly Salary (in USD) - Copy.1"]) + ([#"Q3 - Current Yearly Salary (in USD) - Copy.2.1.2"]) / 2)
    </pre>
    <p>
        All numerical data was then reformatted to <strong>whole numbers</strong> for consistency.
    </p>

    <h2>Languages and Tools Used</h2>
    <ul>
        <li><strong>Power BI</strong></li>
        <li><strong>Power Query (M Language)</strong></li>
        <li><strong>Data Visualization</strong></li>
        <li><strong>Data Cleaning & Transformation Tools</strong></li>
    </ul>

    <h2>Data Preparation Process</h2>
    <ol>
        <li><strong>Column Filtering and Cleaning</strong>
            <ul>
                <li>Removed redundant columns and rows.</li>
                <li>Applied <strong>Split Column</strong> by custom delimiter to isolate components of salary ranges.</li>
                <li>Reformatted data types (e.g., text to numbers).</li>
            </ul>
        </li>
        <li><strong>Calculating Average Salaries</strong>
            <ul>
                <li>Used custom column logic to calculate average salaries from salary ranges.</li>
                <li>Ensured numeric values were uniform for analysis.</li>
            </ul>
        </li>
        <li><strong>Custom Filtering</strong>
            <ul>
                <li>Removed outliers and irrelevant responses based on project goals using text-based filters and transformations.</li>
            </ul>
        </li>
    </ol>

    <h2>Visualizations & Insights</h2>
    <ul>
        <li><strong>Average Salary by Gender</strong>: A comparison of salary distributions across gender groups.</li>
        <li><strong>Average Salary by Job Title</strong>: Identifies which roles tend to earn more on average.</li>
        <li><strong>Job Satisfaction Levels</strong>: Displays survey results indicating satisfaction rates among respondents.</li>
        <li><strong>Survey Respondents by Country</strong>: A global distribution showing where most respondents are located.</li>
        <li><strong>Favorite Programming Languages</strong>: Reveals the most commonly used or preferred languages by survey participants.</li>
    </ul>

    <p>
        This project showcases my ability to clean, transform, and extract meaningful data from real-world survey responses, culminating in a clear and interactive Power BI dashboard.
    </p>

</body>
</html>
