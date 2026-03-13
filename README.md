# Server Monitoring Data Pipeline

## Project Overview
This project implements a data pipeline to monitor server performance and detect resource bottlenecks. The pipeline processes server log data, stores it in a database, and visualizes insights through a Power BI dashboard.

## Architecture
CSV Server Logs → Python Data Processing → SQLite Database → Power BI Dashboard

## Technologies Used
- Python
- Pandas
- SQLAlchemy
- SQLite
- Power BI

## Data Processing Steps
1. Load server log CSV data
2. Convert timestamps
3. Remove duplicate records
4. Create derived metrics:
   - Total Network Traffic
   - Availability
   - High CPU Alert
5. Store processed data in SQLite database

## Dashboard Insights
- Average CPU utilization
- Average memory usage
- Server downtime analysis
- Performance by server location

## Project Structure
server-monitoring-project
│
├── data
│   └── cleanedSample_Data_Ingestion.csv
│
├── scripts
│   └── ingestion_transformation.py
│
├── database
│   └── server_monitoring.db
│
└── dashboard
    └── server_monitoring_dashboard.pbix
