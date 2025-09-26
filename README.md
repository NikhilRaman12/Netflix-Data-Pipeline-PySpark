# Netflix-Data-Pipeline-PySpark
Project Title

Netflix Data Analysis with PySpark

Overview

This project demonstrates end-to-end data analysis using PySpark on the Netflix titles dataset.
It focuses on data cleaning, transformation, exploratory data analysis (EDA), and insights extraction, showcasing the use of PySpark for large-scale data processing along with Pandas, Matplotlib, and Seaborn for visualization.

Objectives

Load and preprocess the Netflix dataset using a defined schema.

Handle missing values and remove duplicate records.

Perform exploratory analysis to uncover trends and patterns.

Identify top genres, directors, and countries contributing to the Netflix library.

Highlight trends in Netflix content releases over the years.

Showcase PySpark’s ability to handle real-world structured data efficiently.

Tech Stack

Language: Python

Big Data Framework: PySpark

Libraries: Pandas, Matplotlib, Seaborn

Environment: Jupyter / Local Machine

Key Steps Implemented

Data Ingestion: Loaded the Netflix dataset (netflix_titles.csv) into a PySpark DataFrame using a predefined schema.

Data Cleaning:

Removed duplicate records

Filled missing values with default placeholders

Filtering & Transformations:

Extracted movies released after 2015 with TV-MA rating

Split and analyzed genre information using explode() and split()

Exploratory Data Analysis (EDA):

Counted titles by type (Movies vs. TV Shows)

Identified top contributing countries and directors

Examined yearly content release trends

Visualization: Converted PySpark results to Pandas DataFrames for generating visualizations.

Data Export: Saved filtered datasets (e.g., post-2015 TV-MA movies, top countries) in CSV format for downstream analysis.

Insights Uncovered

A significant increase in Netflix titles was observed in recent years.

Certain countries consistently dominate the production of Netflix content.

Drama and Comedies remain the most frequent genres.

Several directors repeatedly contribute to Netflix’s movie catalog.

How to Run

Install required dependencies:

pip install pyspark pandas matplotlib seaborn


Place the netflix_titles.csv dataset in the project directory.

Run the Jupyter notebook or Python script to execute the pipeline.

Repository Structure
Netflix_PySpark_Project/
│
├── netflix_pipeline.py
├── netflix_titles.csv
├── output/
│   ├── filtered_movies/
│   └── top_countries/
├── README.md
└── requirements.txt

Future Improvements

Deploy the pipeline on a distributed environment like AWS EMR or Databricks.

Extend the analysis to include NLP on movie descriptions.

Build an interactive dashboard (Tableau / Power BI) connected to processed data.
