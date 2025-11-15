# Play-Store-Analytics-Multi-Source-Data-Integration-EDA
This project was built as part of the Innomatics Research Labs Hackathon. The challenge was to merge three datasets from three different sources and perform deep exploratory data analysis to derive insights about the Google Play Store ecosystem.
# Play Store Unified Analytics – Multi-Source Data Integration & EDA
### By Chidvilas Kumkapalla

---

## Overview
This project was developed as part of the Innomatics Research Labs Hackathon.  
The objective was to integrate datasets from **three different formats** (Excel, JSON, SQLite DB) into a **single unified dataset** and perform comprehensive **Exploratory Data Analysis (EDA)** on Google Play Store applications.

## Copyright Notice:

📄 Dataset used for educational purposes only. All rights reserved to respective owners 
The workflow follows a complete real-world data pipeline:

**Data Integration → Cleaning → Transformation → EDA → Insights**

---

## Project Aim
To merge multiple Play Store datasets into a clean, consistent, analysis-ready DataFrame and generate insights related to:

- App performance  
- Category-wise behavior  
- User sentiment patterns  
- Install and review trends  
- Rating distributions  
- Correlation and temporal insights  

---

## Datasets Used

### 1. Play Store App Data (.xlsx)
Contains app-level metadata:
- App  
- Category  
- Rating  
- Reviews  
- Size  
- Installs  
- Type  
- Price  
- Content Rating  
- Genres  
- Last Updated  
- Current Version  
- Android Version  

### 2. User Reviews Data (.json)
Contains user review text and sentiment information:
- App  
- Translated_Review  
- Sentiment  
- Sentiment_Polarity  
- Sentiment_Subjectivity  

### 3. App Database (.db)
A SQLite database containing additional structured tables such as:
- app_info  
- app_performance  
- review_summary  

---

## Task 1: Data Merging
- Loaded Excel, JSON, and DB tables using Pandas  
- Cleaned and standardized the `App` column to enable accurate merging  
- Combined all datasets using left/right/inner merges where required  
- Resolved inconsistent casing, category mismatches, and missing values  
- Produced a single consolidated DataFrame  

---

## Task 2: Data Cleaning
Performed detailed cleaning operations including:

- Handling missing values in Rating, Reviews, Size, etc.  
- Converting string-based numeric columns (Installs, Price, Reviews) to numeric  
- Standardizing Category, Type, and Content Rating  
- Removing invalid entries (e.g., Rating > 5)  
- Fixing inconsistent text entries  
- Converting size values (KB/MB) into standard MB units  
- Converting Last Updated to datetime format  
- Removing duplicate rows  

Final cleaned dataset stored as:


---

## Task 3: Exploratory Data Analysis (EDA)
Performed visual and statistical analysis to understand:

### Descriptive Insights
- Popular categories  
- Highest rated categories and genres  
- Top-installed applications  
- Distribution of ratings, reviews, installs  

### Sentiment Insights
- Positive, negative, and neutral sentiment distribution  
- Polarity and subjectivity patterns  
- Sentiment vs. rating behavior  

### Correlation Analysis
- Relation between installs, reviews, ratings, size, and price  
- Visualized using correlation heatmaps and scatterplots  

### Temporal Insights
- Update frequency trends  
- Relationship between last update date and app performance  

### Visualizations Used
- Bar charts  
- Line plots  
- Pie charts  
- Histograms  
- Box plots  
- Scatter plots  
- Heatmaps  

---

## Tools and Technologies
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- SQLite  
- JSON processing  
- Jupyter Notebook  

---

## Repository Structure

---

## Key Learning Outcomes
- Merging multi-format datasets using Pandas  
- Performing complex data cleaning and preprocessing  
- Handling real-world inconsistencies and missing data  
- Conducting sentiment-based app analysis  
- Improving visualization and storytelling skills  
- Understanding category-level and sentiment-level insights  
- Strengthening end-to-end data analytics workflow
  

## Conclusion
This project enhanced my ability to work with heterogeneous datasets, clean noisy data, and derive meaningful insights using analytical and visualization skills.  
It reflects real industry-level data engineering and EDA workflows.

