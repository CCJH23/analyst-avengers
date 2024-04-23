# Data Engineering and Full-Stack Web App Project

NOTE: there is no code because the code belongs to the client now.

## Introduction

Created a web application to help client easily check the health status of services and their underlying infrastructure (servers, applications, databases).

The web application provides 3 layers of information -
high-level, mid-level and low-level.

- High-level displays the health status of services.
- Mid-level displays the network of all infrastructure powering that service and a geographical map of where they are located.
- Low-level displays the problem logs of the infrastructure (if it experiences any error) and metric logs.

This web application is powered by a data pipeline ingesting, transforming and loading data every 5 seconds from the monitoring tools.

## Architecture Diagram

<img src="ArchitectureDiagram.png">

## Tech Stack

### Tech Stack for Data Pipeline

- Azure Virtual Machines (deployment of servers, web app, database)
- Prometheus (monitoring tool)
- Zabbix (monitoring tool)
- Apache Nifi (data ingestion)
- Azure Databricks (data transformation)
- Azure Data Lake Gen 2 (raw data storage)
- Azure SQL Database (web app database)

### Tech Stack for Web App

- Vue.JS (frontend)
- Flask (backend)
- Azure SQL database (web app database)
- Pytest (unit and integration testing)
- Github Actions (CI pipeline)
- Firebase (user authentication)
