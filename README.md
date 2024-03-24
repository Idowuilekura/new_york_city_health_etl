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

Data Transformation: The extracted data undergoes necessary transformations to ensure consistency, quality, and compatibility with the target database schema. The transformation is done using Azure Dataflow. The steps taken are
- The first is to use the Data Flow source to get the data from the API
- The second step was to use the select function to select the body content of the response
- The next step was to flatten the content of the body into each column through the derived column function
- The next step was then to filter out null rows from the dataset
- The next was to select the columns

Data Loading: Azure Data Factory's Copy Data activity is employed to load the transformed data into a SQL Azure database.

Data Visualization: Power BI is used to create interactive and visually appealing dashboards and reports based on the loaded data.

Components
Azure Data Factory: Handles the orchestration and automation of the ETL pipeline, including data extraction, transformation, and loading.

SQL Azure Database: Serves as the central repository for storing the transformed health data, allowing for efficient data management and retrieval.
Data Build Tools (DBT): This serves as a data transformation tool in the data warehouse, where transformation and data aggregation for the visualization are made. 
DBT workflow was containerized inside a docker container, and Azure data factory web activity was used to start the container. 

Power BI: Enables the creation of dynamic visualizations and reports to gain insights from the health data, facilitating data-driven decision-making.

Data Flow Workflow 
![image](https://github.com/Idowuilekura/new_york_city_health_etl/assets/38056084/f830da80-3bde-4bb1-b89c-8dd9e9ca19f1)

Data Factory Pipeline 
![image](https://github.com/Idowuilekura/new_york_city_health_etl/assets/38056084/92960272-b426-4208-99f4-8747351c2bb1)



Architectural Diagram 
![image](https://github.com/Idowuilekura/new_york_city_health_etl/assets/38056084/f4e07fd3-c01a-45dd-80c2-50726611823e)


Benefits
Scalability: Azure services offer scalability, allowing the ETL pipeline to efficiently handle large volumes of data.

Automation: Azure Data Factory automates the ETL process, reducing manual intervention and ensuring timely data updates.

Insightful Analysis: Power BI provides powerful visualization capabilities, enabling stakeholders to gain valuable insights from the health data.

![image](https://github.com/Idowuilekura/new_york_city_health_etl/assets/38056084/3d1eec66-4af2-4ebd-9dfe-b879f81d58c5)


The visualization can be accessed through this [link](https://app.powerbi.com/view?r=eyJrIjoiMThmZDE3NDgtNDhkOS00ODQxLWJhNWYtNTQ4NmFmOTBiZDFhIiwidCI6IjJlODZmNjcyLTY3ZGYtNGZjMC04NmE2LWZmZTc4MTY3MTA0ZSIsImMiOjl9)




Conclusion
The New York City Leading Health ETL Pipeline on Azure demonstrates the effective utilization of cloud-based services to streamline the process of collecting, transforming, and visualizing health data. Organizations can make informed decisions to improve public health outcomes by leveraging Azure Data Factory and Power BI.
