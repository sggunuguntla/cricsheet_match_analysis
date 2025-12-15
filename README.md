# Cricsheet Match Data Analysis

## Project Overview
Cricsheet Match Data Analysis is an end-to-end sports analytics project that automates the extraction, processing, analysis, and visualization of cricket match data sourced from **Cricsheet**. The project demonstrates real-world data engineering and analytics skills using **Selenium, Python, SQL, and Power BI** to derive meaningful insights related to player performance, team statistics, and match outcomes.

---

## Project Objectives
- Automate the scraping of cricket match JSON data from Cricsheet
- Transform raw JSON files into clean, structured tabular formats
- Store processed data in a relational SQL database
- Perform analytical SQL queries to extract insights
- Conduct Exploratory Data Analysis (EDA) using Python
- Build interactive Power BI dashboards for data-driven storytelling

---

## Skills & Technologies Used
- **Programming Language:** Python  
- **Web Scraping:** Selenium  
- **Data Processing:** Pandas, JSON  
- **Database:** SQLite / MySQL  
- **Data Analysis:** SQL  
- **Visualization (EDA):** Matplotlib, Seaborn, Plotly  
- **Business Intelligence:** Power BI  
- **Version Control:** Git & GitHub  

---

## Dataset Information
- **Source:** Cricsheet (https://cricsheet.org)
- **Data Format:** JSON (one file per match)
- **Match Types:** Test, ODI, T20, IPL
- **Dataset Includes:**
  - Match metadata (teams, venue, date, toss result)
  - Innings and ball-by-ball delivery data
  - Player batting and bowling statistics

Each JSON file represents an individual cricket match.

## Project Architecture

Cricsheet Website
      ↓
Selenium Web Scraping
      ↓
JSON Files
      ↓
Python Data Processing (Pandas)
      ↓
SQL Database
      ↓
SQL Analysis & Python EDA
      ↓
Power BI Dashboard


## Project Workflow

### 1. Data Scraping (Selenium)
- Automated navigation to https://cricsheet.org/matches/
- Extracted JSON download links using XPath and CSS selectors
- Used Selenium Expected Conditions to handle dynamic content
- Downloaded match data for Test, ODI, T20, and IPL formats

### 2. Data Transformation (Python & Pandas)
- Loaded raw JSON files into Python
- Normalized and flattened nested JSON structures
- Cleaned and formatted data for analysis
- Created separate DataFrames for different match formats

### 3. Database Management (SQL)
- Created an SQL database using SQLite / MySQL
- Designed separate tables for each match type:
  - `test_matches`
  - `odi_matches`
  - `t20_matches`
  - `ipl_matches` (or IPL included under T20 format)
- Inserted cleaned data using SQLAlchemy

### 4. SQL Data Analysis
- Wrote **20 optimized SQL queries** to analyze:
  - Top-performing batsmen and bowlers
  - Team win percentages
  - Match outcome trends
  - Format-wise performance comparisons

### 5. Exploratory Data Analysis (EDA)
- Performed EDA using Matplotlib, Seaborn, and Plotly
- Created **10 meaningful visualizations**, including:
  - Player performance analysis
  - Team comparisons
  - Match outcome distributions
  - Format-wise trends
- Compiled visualizations into a presentation

### 6. Power BI Dashboard
- Connected Power BI to the SQL database
- Built an interactive dashboard with multiple pages:
  - Player Performance Analysis
  - Team Performance Comparison
  - Match Outcomes Analysis
  - Format-wise Comparison
- Added slicers for match type, team, and player for interactivity

## Results & Insights
- Automated extraction of large-scale cricket match data
- Clean and structured SQL database
- Analytical insights derived from SQL queries
- Visual insights from Python-based EDA
- Interactive Power BI dashboard for effective data storytelling
- 
## Project Structure
Cricsheet-Match-Data-Analysis/
1.data/          # Raw and processed JSON data
2.scripts/       # Selenium, data processing, DB scripts
3.sql/           # SQL queries and schema
4.eda/           # EDA notebooks and plots
5.powerbi/       # Power BI dashboard (.pbix)
6.README.md


## Project Deliverables
- Selenium web scraping script
- JSON to DataFrame transformation script
- SQL database and table schemas
- SQL file containing 20 analytical queries
- EDA presentation with visualizations
- Power BI dashboard (.pbix)
- Detailed project documentation

## Evaluation Metrics
- Accuracy and completeness of scraped data
- Correctness and efficiency of SQL queries
- Quality and clarity of Power BI dashboards
- Seamless integration of Selenium, Python, SQL, and Power BI
- Relevance and clarity of insights presented

## Conclusion
This project showcases a complete data analytics pipeline using real-world sports data. It highlights automation, data engineering, analytical thinking, and visualization skills that are highly relevant for data analyst and data engineer roles.
