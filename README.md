<h1>Power BI Data Professionals Dashboard</h1>

<h2>Description</h2>
The <strong>Data Professionals Dashboard</strong> is a Power BI project that focuses on analyzing and visualizing survey data from individuals in various data-related roles. The goal was to clean the dataset, extract useful insights, and present the findings in an interactive and informative dashboard.

This project demonstrates <strong>data cleaning and transformation</strong>, <strong>custom column creation using Power Query</strong>, and <strong>data visualization in Power BI</strong>.

<br />

<h2>Languages and Tools Used</h2>

- <b>Power BI</b>
- <b>Power Query (M Language)</b>
- <b>Custom Column Logic</b>
- <b>Data Modeling</b>
- <b>Interactive Dashboards</b>

<h2>Data Preparation and Transformation</h2>

1. <strong>Removing Unnecessary Columns:</strong>
   - Used the <code>Remove Columns</code> feature to discard irrelevant data.
   - Applied filters to remove rows with missing or invalid entries that didn't align with project goals.

2. <strong>Splitting Salary Ranges:</strong>
   - The original salary column was in the format <code>50k-60k</code>.
   - Used <code>Split Column</code> by custom delimiter to separate the lower and upper salary values into two columns.

3. <strong>Creating Average Salary Column:</strong>
   - A new custom column was created to calculate the average between the two salary values.
   - The formula used in Power Query:
     <pre>
= Table.AddColumn(#"Removed Columns7", "Average", each ([#"Q3 - Current Yearly Salary (in USD) - Copy.1"]) + ([#"Q3 - Current Yearly Salary (in USD) - Copy.2.1.2"]) / 2)
     </pre>
   - Reformatted the values as whole numbers for consistency and easier analysis.

<h2>Insights and Visualizations</h2>

- <b>Average Salary by Gender:</b> Visualized salary distribution across different gender identities.
- <b>Average Salary by Job Title:</b> Identified which roles offer higher pay on average.
- <b>Job Satisfaction Levels:</b> Analyzed how satisfied respondents were with their current roles.
- <b>Respondents by Country:</b> Showed the geographic distribution of survey participants.
- <b>Favorite Programming Language:</b> Visualized the most commonly preferred languages by professionals.

<br />

<h2>Conclusion</h2>

This Power BI project showcases my ability to handle real-world datasets—from cleaning and transforming complex inputs to extracting meaningful insights using visual storytelling. The final dashboard provides a comprehensive overview of key patterns within the data professional community.
