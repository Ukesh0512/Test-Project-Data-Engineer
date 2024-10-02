# Test-Project-Data-Engineer
# Data Pipeline

# Marketing Data Pipeline Project

## Overview

This project creates a data pipeline to extract, transform, and load marketing data into a database. The pipeline is designed to handle social media engagement, email campaign performance, and web traffic metrics.

## Setup

1. Clone the repository: `git clone https://github.com/username/marketing-data-pipeline.git`
2. Install dependencies: `pip install -r requirements.txt`
3. Create a SQLite database: `sqlite3 marketing_data.db`
4. Run the data pipeline script: `python data_pipeline.py`

## Assumptions

* The CSV files are in the same directory as the script.
* The database is a SQLite database.
* The data is in the correct format (e.g., dates are in YYYY-MM-DD format).

## Design Decisions

* We used a SQLite database for simplicity and ease of use.
* We used the `pandas` library for data manipulation and `sqlalchemy` for database interactions.
* We aggregated daily traffic metrics by week to reduce data size and improve query performance.

## Bonus Tasks

* Automation: We used the `schedule` library to automate the pipeline to run daily at midnight.
* Data Visualization: We used Google Data Studio to create a dashboard to visualize the data.

## Future Improvements

* Add more data sources (e.g., customer feedback, sales data).
* Improve data quality checks and error handling.
* Use a more robust database (e.g., PostgreSQL, MySQL).

## requirements.txt

* pandas
* sqlalchemy
* schedule
* google-auth
* google-api-python-client
