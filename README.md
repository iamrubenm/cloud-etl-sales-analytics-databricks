Data Transformation and Analysis (Databricks Project)

Overview
This project demonstrates the end-to-end pipeline for transforming, storing, and analyzing the Adventure Works dataset using Databricks and Azure Data Lake. The workflow covers data extraction, transformation, storage optimization, and sales analysis with visualization.

Project Steps
1. Data Extraction
Source: Adventure Works CSV files stored in Azure Data Lake (Bronze Layer).

Method: CSV files were ingested into Databricks notebooks by connecting to Azure Data Lake Storage.

2. Data Transformation
CSV data underwent necessary cleaning, type casting, and normalization steps.

Redundant and inconsistent fields were handled to ensure data quality.

Complex transformations such as joins, aggregations, and derived columns were applied as needed.

3. Data Storage
Target: Azure Data Lake (Silver Layer).

Format: Transformed datasets saved in Parquet format for optimal performance and compression.

This enhances query performance for downstream analytics and reduces storage costs.

4. Sales Data Analysis
Exploratory Data Analysis (EDA): Focused on the sales dataset to uncover key metrics and trends.

Visualizations (bar charts, line graphs, etc.) were created within Databricks to highlight sales performance, top-selling products, and seasonal trends.

Insights were drawn into sales distribution, product popularity, and regional contributions.

How to Use
Prerequisites: Access to Azure Data Lake, Databricks Workspace, and Adventure Works dataset in CSV format.

Data Loading: Use the provided notebooks/scripts to pull the raw CSV data from your Azure Data Lake Bronze container.

Transformation: Execute the transformation workflows to process and clean the data.

Storage: Save processed data as Parquet files in the Silver container of Azure Data Lake.

Analysis: Run the included analysis scripts/notebooks to visualize the sales dataset and extract insights.

Project Structure
notebooks/: Contains Databricks notebooks for extraction, transformation, and analysis.

data/bronze/: Raw CSV files.

data/silver/: Transformed Parquet files.

visualizations/: Sample charts and plots from sales analysis.

Key Technologies
Databricks

Azure Data Lake Storage (ADLS)

PySpark

Parquet Format

Results
Cleaned and optimized Adventure Works dataset available in Parquet format in your Azure Data Lake "Silver" layer.
Informative visualizations and actionable insights on sales data.
