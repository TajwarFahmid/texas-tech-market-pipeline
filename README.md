🚀 2026 Texas Tech Market Intelligence Pipeline
An end-to-end Data Engineering & Analytics project tracking the Data Science and Software Engineering landscape across the Texas Triangle.

📊 Executive Summary
This project architected a live data pipeline to monitor hiring trends in Dallas-Fort Worth, Austin, and Houston. By scraping real-time job data and enriching it with 2026 market benchmarks, I uncovered key insights into salary variances and seniority demands across the region.

Key Market Insights:

Hiring Giants: Major players like TELUS Digital and Walmart dominate the volume, specifically in the DFW metroplex.

Seniority Skew: Over 51% of active roles are categorized as Senior Level, highlighting a high barrier to entry in the current market.

The "Austin Premium": While Dallas leads in job volume, Austin maintains a significant lead in average annual compensation for Software Engineering roles.

🛠️ The Tech Stack
Extraction: Python (Requests, BeautifulSoup)

Data Warehouse: PostgreSQL (Cloud-hosted via Neon)

Logic & Cleaning: Advanced SQL (Views, CASE statements, Joins)

Visualization: Tableau Public

📂 Project Architecture & Repository Structure
texas_tech_market_scraper.py: Python ETL script that extracts raw data from The Muse API.

sql_queries: SQL scripts containing the database schema, data cleaning views, and the logic for salary enrichment.

v_final_jobs.xlsx: The final, cleaned, and enriched dataset used for visualization.

2026 Texas Job Market for Data/Software Engineering: The Tableau Packaged Workbook (.twbx) for offline viewing.

⚙️ How it Works
Ingestion: The Python scraper collects raw JSON data including job titles, locations, and categories.

Transformation: Using SQL Views, I filtered out non-tech "noise" (like retail/service roles) and normalized seniority levels into four clean buckets: Internship, Junior/Entry, Mid-Level, and Senior.

Enrichment: I performed a LEFT JOIN between the job listings and a custom Salary Benchmark table to assign market-accurate compensation estimates.

Delivery: The cleaned data was connected to Tableau to create an interactive marketplace report.

📈 Dashboard Preview
(https://github.com/TajwarFahmid/texas-tech-market-pipeline/blob/main/Dashboard%201.png)
