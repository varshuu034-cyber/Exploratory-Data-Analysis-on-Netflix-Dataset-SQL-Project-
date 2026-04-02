# Exploratory-Data-Analysis-on-Netflix-Dataset-SQL-Project-
Add More SQL Questions
Example queries:
SQL
-- Top 10 directors with most Netflix titles
SELECT director, COUNT(*) AS total_titles
FROM netflix_titles
WHERE director IS NOT NULL
GROUP BY director
ORDER BY total_titles DESC
LIMIT 10;
-- Average movie duration
SELECT AVG(CAST(REPLACE(duration,' min','') AS INT)) AS avg_duration
FROM netflix_titles
WHERE type='Movie';
Add These Files in GitHub
Create repository like:

Netflix-SQL-Analysis
│
├── dataset.csv
├── sql_queries.sql
├── project_report.pdf
└── README.md
README should include:
Project overview
Dataset source (Kaggle)
SQL queries
Key insights
Screenshots of output
Add Visualization (Optional but Powerful)
Use:
Python (Matplotlib)
Power BI
Excel charts
Example:
Movies vs TV shows chart
Top countries chart
Yearly content growth chart
