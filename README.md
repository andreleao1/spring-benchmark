# Spring Benchmark Test

## Description

This project aims to demonstrate the impact of non-normalized data models on API performance. The implementation involves two versions: one using denormalized data and the other using normalized data. We will perform stress testing with JMeter and analyze the results using Grafana. The application is a Java-based API using Spring, which connects to a PostgreSQL database.

## Technologies Used

- **Java 21**
- **Spring 3.4.3**
- **Docker**
- **Prometheus**
- **Grafana**

## How to Run the Project Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/andreleao1/spring-benchmark.git
2. Navigate to the project directory:
    ```bash
   cd spring-benchmark
3. Run Docker Compose to start the application and services:
   ```bash
   docker compose up -d
   ```
   this will start the PostgreSQL, Prometheus, and Grafana containers.
4. Once the containers are up and running, you can run the application and access it at http://localhost:8080

## Accessing and Importing the Dashboard JSON in Grafana

1. Open Grafana in your browser at: http://localhost:3000

2. On the first login, use the default credentials:
    - **Username**: admin
    - **Password**: admin

3. You will be prompted to change the password. Choose a password of your preference.

4. Once logged in, navigate to the Dashboards section:
   - Go to the URL: http://localhost:3000/dashboards

5. Click on the **New** button located at the top right corner.

6. Select **Import** from the dropdown menu, or go directly to:
   - http://localhost:3000/dashboard/import

7. Click on the **Upload dashboard JSON file** option and select the dashboard.json file located in the dashboards directory of the project.

8. After importing the JSON file, you should be able to view the performance metrics and graphs on the Grafana dashboard.