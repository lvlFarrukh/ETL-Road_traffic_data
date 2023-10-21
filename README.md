![image](https://github.com/lvlFarrukh/ETL-Road_traffic_data/assets/47663235/6839fdc0-4041-4300-9883-106f180908f5)# ETL Project: National Highway Traffic Data Analysis

## Overview

This project aims to de-congest the national highways by analyzing road traffic data from different toll plazas. Each highway is operated by a different toll operator with a different IT setup that uses various file formats. The goal is to collect data available in different formats and consolidate it into a single file for analysis.

### Project Components

- **DAGs (`dags/`)**: Apache Airflow DAG definition files for orchestrating ETL tasks.

- **Scripts (`scripts/`)**: Bash scripts and Python scripts for data extraction, transformation, and loading.

- **Data (`data/`)**: Raw data collected from different toll plazas. You can get this data from this link https://cf-courses-data.s3.us.cloud-object-storage.appdomain.cloud/IBM-DB0250EN-SkillsNetwork/labs/Final%20Assignment/tolldata.tgz

- **Requirements (`requirements.txt`)**: List of Python dependencies for the project.

## Usage

1. Set up Apache Airflow and configure it using `airflow.cfg`.
2. Ensure you have Apache Kafka set up and configure the connection in `kafka_config.json`.
3. Customize the DAG in `dags/your_dag.py` to define your ETL workflow.
4. Modify the scripts in `scripts/` to handle data extraction, transformation, and loading.
5. Run your ETL process using Airflow.

## Getting Started

To get started with this project, follow these steps:

1. Clone this Git repository.

2. Install the required Python packages using `pip install -r requirements.txt`.

3. Set up Apache Airflow and Apache Kafka with your specific configurations.

4. Customize the project components to match your data sources, transformations, and loading requirements.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these guidelines:

- Fork the repository.

- Create a new branch for your feature or bug fix.

- Make your changes and submit a pull request.

## Contact

For questions or feedback, please contact [Farrukh Aslam](mailto:farrukha303@gmail.com).

Happy data engineering!

## Usefull Commands

- sudo mkdir -p /home/project/airflow/dags/finalassignment/staging
- cd /home/project/airflow/dags/finalassignment
  
- cp .py $AIRFLOW_HOME/dags
- airflow dags list
- airflow dags list|grep "my-first-dag"
- airflow tasks list my-first-dag

- bin/zookeeper-server-start.sh config/zookeeper.properties  ( run zookeeper server )
- bin/kafka-server-start.sh config/server.properties  ( run kafka broker server )
- bin/kafka-topics.sh --create --topic news --bootstrap-server localhost:9092 ( create topic )

