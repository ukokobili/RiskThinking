# Stock Market Data Pipeline with DAG-Oriented Tool and ML Integration

## Project Description
The objective of this project is to build a data pipeline to process, transform and analyze stock market data using DAG-oriented tools and integrate an ML predictive model training step into the pipeline. The project consists of four problems, where each problem is a separate task in the pipeline.

## Table of Contents
*   [Installation]()
*   [Usage]()
*   [Credits]()
*   [License]()

## Installation

The following are the steps required to install the project and get the development environment running:

1. Clone the repository

`https://github.com/ukokobili/RiskThinking`

2. Install Docker

Find details for Docker installation [here](https://www.docker.com/products/docker-desktop/)

3. Setup Airflow
Create `dag`, `logs`, `plugins`, `load`, `stage` and `model` folders in the working directory.

`mkdir -p ./dags ./logs ./plugins ./load ./stage ./model
echo -e "AIRFLOW_UID=$(id -u)" > .env`

Make sure to mouht `load`, `stage` and `model` path to `volume` in the `docker-compose.yaml` file. More details on how to setup Airflow with `docker-compose` [here](https://github.com/DataTalksClub/data-engineering-zoomcamp/blob/main/cohorts/2022/week_2_data_ingestion/airflow/1_setup_official.md).

3. Download the dataset from [source](https://www.kaggle.com/datasets/jacksoncrow/stock-market-dataset.)
After setting up Airflow
    
