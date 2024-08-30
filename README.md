# Microsoft Azure Data Fundamentals DP-900 Exam Prep
I'm currently enrolled in the DP-900 Exam Prep course on [Coursera](https://www.coursera.org/specializations/microsoft-azure-dp-900-data-fundamentals), and this notebook contains my personal notes that I am using to prepare for the DP-900 certification. </br>
I hope these notes can be useful to others who are also studying for this certification. </br>
Note: you can study for free at [Learn Microsof](https://learn.microsoft.com/en-us/credentials/certifications/azure-data-fundamentals/?practice-assessment-type=certification). 

#########################################################################

# Skills Measured
I wrote down here in this section everything that we have to know to get the DP-900 certificate. Important to say the exam has between 40-60 questions (120 min of duration) and we need to reach 700 points (70%) to pass it. And the exam is divided by:
## Describe core data concepts (15-20%)
### Types of core data workloads
- streaming data
- differente between batch and streaming data
- characteristics of relational data
### Data analytics core concepts
- data visualization (visualization, reporting, business intelligence)
- basic chart types (bar and pie)
- analytics techniques (descriptive, diagnostic, predictive, prescriptive, cognitive)
- describe ELT and ETL processing
- describe the concepts of data processing

## Describe how to work with relational data on Azure (25-30%)
### Relational data workloads
- Right data offering for a relational workload
- Relational data structures (tables, index, views)
### Azure data services
- Difference between PaaS, IaaS, and SaaS solutions
- Azure SQL database services (Azure SQL Database, Azure SQL Managed Instance, and SQL Service on Azure Virtual Machine)
- Azure Synapse Analytics
- Azure Database for PostgreSQL, Azure Database for MariaDB, and Azure Database for MySQL
### Basic management tasks for relational data
- Provisioning and deployment of relational data services
- Methor for deployment including the Azure portal, Azure Rescourse Manager temmplates, Azure PowerShell, and the Azure command-line interface (CLI)
- Data security components (firewall, authentication)
- Basic connectivity issues (accessing from on-premises, access with Azure VNets, access from Internet, authentication, firewalls)
- Query tools (Azure Data Studion, SQL Server Management Studio, sqlcmd utility, etc)
### Query techniques for data using SQL Language
- Compare Data Definition Language (DDL) x Data Manipulation Language (DML)
- Query relational data in Azure SQL Database, Azure Database for PostgreSQL, and Azure Database for MySQL

## Describe how to work with non-relational data on Azure (25-30%)
### Describe non-relational data workloads
- Characteristics of non-relational data
- Types of non-relational and NoSQL data
- Recommend the correct data store
- When to use non-relational data
### Non-relational data offering on Azure
- Identify Azure data services for non-relational workloads
- Azure Cosmos DB APIs
- Azure Table storage
- Azure Blob storage
- Azure File storage
### Basic management tasks for non-relational data
- Provisioning and deployment of non-relational data services
- Method for deployment including the Azure portal, Azure Resource Manager templates, Azure PowerShell, and the Azure command-line interface (CLI)
- Data Security components (firewall, authentication, encryption)
- Basic connectivity issues (accessing from on-premises, access with Azure VNets, access from Internet, authentication, firewalls)
- Management tools for non-relational data
## Analytics workload on Azure (25-30%)
### Describe Analytics workloads
- Transactional Workloads
- Difference between Transactional and Analytics worklaods
- Difference between Batch and Real Time
- Data warehousing workloads
- When a data warehouse solution is needed
### Describe the components of a modern data warehouse
- Azure data services for modern data warehousing such as Azure Data Lake, Azure Synapse Analytics, Azure Databricks, and Azure HDInsight
- Modern data warehousing architecture and workload
### Describe data ingestion and processing on Azure
- Commom practices for data loading
- Components of Azure Data Factory (pipeline, activities, etc)
- Data processing options (Azure HDInsight, Azure Databricks, Azure Synapse Analytics, Azure Data Factory)
### Describe data visualization in Microsoft Power BI
- Role of paginated repoting
- Role of interactive Reports
- Role of Dashboards
- Workflow in Power BI

#########################################################################
# 1. Core Data Concepts
## 1.1 Types of Core Data Workload 
### Streaming data
### Differente between Batch and Streaming data
### Characteristics of Relational Data
We have basic three types of data and for every ocasion, Azure has also differets services to runs it in the cloud.
- Structured: It's typically Tabular Data, that is represented by rows and columns in a database.
Azure service to runs structured data is called [*Azure SQL Database* ](https://learn.microsoft.com/en-us/azure/azure-sql/database/sql-database-paas-overview?view=azuresql)
- Semi-structured: It's information that doens't resid in a relational database but it still has some structure to it. It's normally extensions in JavaScript or JSON format.
Azure service: [*Azure Cosmos DB*](https://learn.microsoft.com/en-us/azure/cosmos-db/introduction)
- Unstructured: It's data which contains every kind of midia such as Audios, Videos and Images, it's also considered unstructured data Binary files.
For this files, they are storage at [*Azure Blob Storage*](https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blobs-introduction) (Blob = Binary Large Object)
  
## 1.2 Data Analytics Core concepts
### Data visualization
### Basic chart types
### Analytics techniques
### ELT and ETL processing
### Concepts of data processing

# 2. Relational data on Azure
## 2.1 Relational data workloads
### Right data offering for a relational workload
### Relational Data Structures (tables, index, views)
Structure Data is basic the tables that we're used to work, where each row in a table has the same set of columns.   
  
## 2.2 Azure data services
### Difference between PaaS, IaaS, and SaaS solutions
### Azure SQL database services (Azure SQL Database, Azure SQL Managed Instance, and SQL Service on Azure Virtual Machine)
### Azure Synapse Analytics
### Azure Database for PostgreSQL, Azure Database for MariaDB, and Azure Database for MySQL
  
## 2.3 Basic management tasks for relational data
### Provisioning and deployment of relational data services
### Methor for deployment including the Azure portal, Azure Rescourse Manager temmplates, Azure PowerShell, and the Azure command-line interface (CLI)
### Data security components (firewall, authentication)
### Basic connectivity issues (accessing from on-premises, access with Azure VNets, access from Internet, authentication, firewalls)
### Query tools (Azure Data Studion, SQL Server Management Studio, sqlcmd utility, etc)
  
## 2.4 Query techniques for data using SQL Language
### Compare Data Definition Language (DDL) x Data Manipulation Language (DML)
### Query relational data in Azure SQL Database, Azure Database for PostgreSQL, and Azure Database for MySQL

# 3. Describe how to work with non-relational data on Azure (25-30%)
## 3.1 Describe non-relational data workloads
### Characteristics of non-relational data
### Types of non-relational and NoSQL data
### Recommend the correct data store
### When to use non-relational data
  
## 3.2 Non-relational data offering on Azure
### Identify Azure data services for non-relational workloads
### Azure Cosmos DB APIs
### Azure Table storage
### Azure Blob storage
### Azure File storage
  
## 3.3 Basic management tasks for non-relational data
### Provisioning and deployment of non-relational data services
### Method for deployment including the Azure portal, Azure Resource Manager templates, Azure PowerShell, and the Azure command-line interface (CLI)
### Data Security components (firewall, authentication, encryption)
### Basic connectivity issues (accessing from on-premises, access with Azure VNets, access from Internet, authentication, firewalls)
### Management tools for non-relational data
  
# 4. Analytics Workload on Azure 
## 4.1 Describe Analytics workloads
### Transactional Workloads
It's often what most people consider the primary function of business computing.
It can be Financial, Retail system, it contains a High-volume (it's possible to run millions transactions in a day), Online Transaction Processing (OLTP)
### Difference between Transactional and Analytics worklaods
### Difference between Batch and Real Time
### Data warehousing workloads
### When a data warehouse solution is needed
  
## 4.2 Describe the components of a modern data warehouse
### Azure data services for modern data warehousing such as Azure Data Lake, Azure Synapse Analytics, Azure Databricks, and Azure HDInsight
### Modern data warehousing architecture and workload
  
## 4.3 Describe data ingestion and processing on Azure
### Commom practices for data loading
### Components of Azure Data Factory (pipeline, activities, etc)
### Data processing options (Azure HDInsight, Azure Databricks, Azure Synapse Analytics, Azure Data Factory)
  
## 4.4 Describe data visualization in Microsoft Power BI
### Role of paginated repoting
### Role of interactive Reports
### Role of Dashboards
### Workflow in Power BI




