# Scheduling Python Code on Cloud Foundry

## Overview

This project demonstrates how to schedule and execute Python scripts on Cloud Foundry using a scheduler service. It enables automation of recurring tasks such as data processing, report generation, API integrations, monitoring, and ETL workflows without manual intervention.

## Features

* Automated execution of Python scripts on predefined schedules
* Cloud-native deployment using Cloud Foundry
* Easy configuration through `manifest.yml`
* Dependency management using `requirements.txt`
* Runtime specification through `runtime.txt`
* Logging and monitoring support for scheduled jobs

## Project Structure

```text
Scheduling-Python-code-on-Cloud-Foundry/
│
├── hana_ml_credstore.py   # Main Python script
├── manifest.yml           # Cloud Foundry deployment configuration
├── requirements.txt       # Python dependencies
├── runtime.txt            # Python runtime version
└── README.md              # Project documentation
```

## Prerequisites

* Cloud Foundry CLI installed
* Access to a Cloud Foundry environment
* Python 3.x
* Scheduler service enabled in your Cloud Foundry space

## Deployment

1. Clone the repository:

```bash
git clone https://github.com/<your-username>/Scheduling-Python-code-on-Cloud-Foundry.git
cd Scheduling-Python-code-on-Cloud-Foundry
```

2. Deploy the application:

```bash
cf push
```

3. Bind the scheduler service to the application.

4. Create a scheduled job using the Cloud Foundry scheduler:

```bash
cf create-job <app-name> <job-name> "<command>"
```

## Use Cases

* Automated data ingestion pipelines
* Scheduled database operations
* API data synchronization
* Report generation
* Monitoring and maintenance tasks
* ETL workflow automation

## Technologies Used

* Python
* Cloud Foundry
* Cloud Foundry Scheduler
* SAP HANA ML (if applicable)

## Author

Saket Gudimella
