# Data Ingestion Pipeline

## Overview

This project involves building a comprehensive data ingestion pipeline that integrates both **batch data migration** and **real-time streaming data ingestion**. The pipeline uses tools like **Apache Sqoop**, **Apache Flume**, and **Apache Kafka** to ensure efficient data handling. The project is designed to handle both historical data and real-time streaming data, providing a robust and scalable solution for data ingestion.

## Features

- **Batch Data Migration**: Transfer historical data from MySQL to Hadoop HDFS using Apache Sqoop.
- **Real-Time Data Ingestion**: Use Apache Flume to capture and move log data into Apache Kafka for real-time processing.
- **Incremental Data Import**: Utilize append mode for incremental data import, ensuring that only new data is added.

## Objectives

1. Migrate historical data from a relational database to Hadoop HDFS.
2. Capture and ingest real-time data from a local directory, simulating continuous data flow.
3. Ensure seamless data integration between batch and streaming data sources.

## Tools and Technologies

- **Apache Sqoop**: For batch data migration from MySQL to HDFS.
- **Apache Flume**: For real-time data ingestion from a local directory to Kafka.
- **Apache Kafka**: For buffering and streaming real-time data.
- **Hadoop HDFS**: Storage layer for both batch and streaming data.

## Setup and Usage

### 1. Batch Data Ingestion (Apache Sqoop)

- **Environment Setup**: Install Hadoop and MySQL on your local machine or cluster.
- **Database Preparation**: Prepare the MySQL database for migration.
- **Data Migration**: Use Apache Sqoop to import the data into HDFS.
- **Incremental Import**: Ensure continuous data flow by appending only new rows to HDFS.

### 2. Real-Time Data Ingestion (Apache Flume & Kafka)

- **Environment Setup**: Install and configure Apache Flume and Kafka.
- **Log File Setup**: Create a logs directory and generate log files for ingestion.
- **Flume Configuration**: Set up Flume to monitor and capture log data.
- **Kafka Configuration**: Set up a Kafka topic to manage and store incoming data.
