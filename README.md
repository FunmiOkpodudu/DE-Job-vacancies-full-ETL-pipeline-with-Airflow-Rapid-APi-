PROJECT TITLE - AIRFLOW PIPELINE_PROJECT using python Operator

Project Overview

The Data Engineering Job Vacancies ETL Pipeline aims to automate the process of gathering relevant job vacancy data from a RapidAPI service, performing data transformations, and storing the processed data in a PostgreSQL database. The structured data is enriched with extracted skills from the job descriptions, providing valuable insights into the sought-after skills in the job market.

How it Works
Data Extraction: The pipeline queries a reputable RapidAPI endpoint to fetch up-to-date job vacancies for data engineering positions in Ontario, Canada. The data is fetched daily to ensure real-time information.

Data Transformation: The extracted data is meticulously processed and transformed into a structured DataFrame. As a unique feature, this pipeline identifies essential skills from the job descriptions using predefined lists and categorizes them accordingly.

Data Loading: The structured and enriched data is securely loaded into a dedicated PostgreSQL database table named "new_rapid_api_jobs1." The PostgreSQL database acts as a centralized repository for easy access and analysis.

Requirements
Python 3.x
Airflow
Requests
Pandas
SQLAlchemy
PostgreSQL

Usage
- Code already been modified from the github account by retriving the task using git bash command prompt. 

- Start up Airflow as configured in the docker-compose.yaml file using docker-compose up -d in VS code(some little modification was made like changing the ports, name of the owner)

- Set up a PostgreSQL database with credentials and ensure the connection URL is correctly provided in the script.

- Create a RapidAPI account and obtain an API key for accessing the job vacancy data.


- Run the pipeline with Airflow using the provided DAG, ensuring that the required connections and variables are properly configured.

Contribution and Feedback

This project has helped me to learn more by using several requiremnts needed to practice ETL techniques with airflow. 

Airflow offers ability to scehdule, monitor, and most importantly, scale, increasingly complex workflows.
