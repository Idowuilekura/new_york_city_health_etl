# New York City Leading Health ETL Pipeline on Azure
This project focuses on developing an Extract, Transform, Load (ETL) pipeline using Azure services to gather health-related data for New York City and visualize it using Power BI.

## Overview
This project aims to create an efficient ETL pipeline to collect health data from various sources, transform it, and load it into a SQL Azure database. The collected data is then visualized using Power BI for insightful analysis and decision-making.

Technologies Used
- Azure Data Factory
- SQL Azure
- Power BI

### Workflow
Data Extraction: Azure Data Factory is utilized to fetch data from REST APIs providing health-related information for New York City.

Data Transformation: The extracted data undergoes necessary transformations to ensure consistency, quality, and compatibility with the target database schema.

Data Loading: Azure Data Factory's Copy Data activity is employed to load the transformed data into a SQL Azure database.

Data Visualization: Power BI is used to create interactive and visually appealing dashboards and reports based on the loaded data.

Components
Azure Data Factory: Handles the orchestration and automation of the ETL pipeline, including data extraction, transformation, and loading.

SQL Azure Database: Serves as the central repository for storing the transformed health data, allowing for efficient data management and retrieval.

Power BI: Enables the creation of dynamic visualizations and reports to gain insights from the health data, facilitating data-driven decision-making.

Architectural Diagram 
![image](https://github.com/Idowuilekura/new_york_city_health_etl/assets/38056084/bb670d95-87ce-4c84-954d-7cb87d4ffbc5)


Benefits
Scalability: Azure services offer scalability, allowing the ETL pipeline to efficiently handle large volumes of data.

Automation: Azure Data Factory automates the ETL process, reducing manual intervention and ensuring timely data updates.

Insightful Analysis: Power BI provides powerful visualization capabilities, enabling stakeholders to gain valuable insights from the health data.

![image](https://github.com/Idowuilekura/new_york_city_health_etl/assets/38056084/3d1eec66-4af2-4ebd-9dfe-b879f81d58c5)


The visualization can be accessed through this [link](https://app.powerbi.com/view?r=eyJrIjoiMThmZDE3NDgtNDhkOS00ODQxLWJhNWYtNTQ4NmFmOTBiZDFhIiwidCI6IjJlODZmNjcyLTY3ZGYtNGZjMC04NmE2LWZmZTc4MTY3MTA0ZSIsImMiOjl9)




Conclusion
The New York City Leading Health ETL Pipeline on Azure demonstrates the effective utilization of cloud-based services to streamline the process of collecting, transforming, and visualizing health data. Organizations can make informed decisions to improve public health outcomes by leveraging Azure Data Factory and Power BI.
