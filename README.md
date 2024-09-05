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
Depending on how the data is ingested into the system, we can process each data item as it arrives. Buffering and processing data in groups is called *Batch*, in the other way, *Streaming data* is called when it process in the real time.
- Batch: Each new data elements are colleted into a group. So you can process data elements based on time or as a result of some event. </br>
e.g. Votes conted in election.
- Streaming Data: Each piace of data is process when it arrives. So, it process in real-time. </br>
e.g. Online gaming company, Financial institution, Real-estate website. 

### Characteristics of Relational Data
All data is tabluar, entities are modeled as tables; All rows have the same set of column; A table can contain any number of rows; PK is unique indetifier; FK refers to a row in another related table. </br>
In relational database, you model collections of entities from the real world as tables. (Entity: A thing about which information needs to be known.) </br>
Primary Key (PK) indicates the column that uniquely indentify each row, every table should have one. </br> 
Foreign Key (FK) is used to maintain the relationship between tables. </br>

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
Relational Database Management Systems (RDMBS): 
- Scalability: 
- Balance: 
- Data valuation:
- Security:

### Relational Data Structures (tables, index, views)
- Index: Helps to search for a data in a table;
- Some relational database management systems also support clustered indexes. A clustered index physically reorganizes a table by the index key.

- View: It's a virtua table based on the results set of a query.

Structure Data is basic the tables that we're used to work, where each row in a table has the same set of columns.   
  
## 2.2 Azure data services
### Difference between PaaS, IaaS, and SaaS solutions
You can hold your database in different ways on Azure: 
- [IaaS](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-iaas/) (Infrastructure-as-a-Service): 
Azure enables us to create Virtual infrastructure in the cloud; Virtual machines & networks; and it's the user's responsable for software installation & maintenance.
 
- [PaaS](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-paas/) (Platform-as-a-Service):
Rather than creating a virtual infrastructure and installing and managing the database software by yourself, a PaaS solution does it for us. The user has to Specify the resources that they require, then, Azure atumatically creates the virtual infrastructure necessary, the user also can scale up and down as their needs.
Azure SQL Database; Azure Database for PostgreSQL; Azure Database for MySQL; Azure Database for MariaDB

- [SaaS](https://azure.microsoft.com/en-us/resources/cloud-computing-dictionary/what-is-saas/) (Software-as-a-Service):
Typically hosted applications rather than more generalized software such as DBMS. Common SaaS packages available on Azure include MS365. 

IaaS's the most flexible category of Cloud Services. It allows the user the complete control over the hardware that runs thei application. PaaS provide the same thing but there are some additional benefits, such as database management and operating systems. SaaS has everything mentioned but again, it has some additioanl benefits as Hosted applications. 
SaaS>PaaS>IaaS

### Azure SQL database services (Azure SQL Database, Azure SQL Managed Instance, and SQL Service on Azure Virtual Machine)
- *Azure SQL Database*: The user create a managed databased server in the Cloud, and then deploy their databases on the server. It has several options to use Azure SQL Database:
    1. [Single Database](https://docs.microsoft.com/en-us/azure/azure-sql/database/single-database-overview): Set and runa a single SQL Server database. It scales up and down automatically or with the user needs. </br> 
    2. Elastic Pool (Pool is a reference to resources): Multiple databases can share de same resource such as memory, storage and processing power.  </br>
    3. Managed Instance: High compatibility with SQL Server </br>
- *Azure SQL Database Managed Instance*: Manages instance effectively run a fully controllable instance of SQL server in the cloud. The user can install multiple databases on same instance, and also they have all control under them. 

### Azure Synapse Analytics


### Azure Database for PostgreSQL, Azure Database for MariaDB, and Azure Database for MySQL
Relational dataases systems:
 - MySQL: It's the most frequently used by commercial organizations, althought have versions of MySQL aren't free.
 - MariaDB: Newer DBMS created by the same developers as MySQL. The newest tool is that they built-in support for temporar data, so a table can hold serveral versions of data.
 - PostgreSQL: Hybrid relational-object database. Hybrid means it can store both relational and non-relational data. Storage and manipulation of geometric data. It has their own language, called pgsql. PostgreSQL has two deployment options, Single-server and Hyperscale: </br>
     1. Azure Database for PostgreSQL single-server: The user can choose between 3 pricing tiers where each tier has different numbers of cpus memory and storage sizes. </br>
     2. Azure Database for PostgreSQL Hyperscale (Citus): Database split across nodes, data split into chunks based on key value and useful for largest cloud deployment. </br>

To migrate the data do a database running the mentionend data services, you can use Azure Database Migration Service (DMS)
  
## 2.3 Basic management tasks for relational data
### Provisioning and deployment of relational data services
*Provising* is the act of running a series of tasks to create, configure, and make available a service, such as Azure SQL database.
The service provider will set up various resources such as Disks, Memory, CPUs network. The user will be assigned these resources and they remain allocated to them and charged until they delete the service. It's not our concern how this process works, but the user has to specify parameters which will determine the size of the resources required, the user can also modify these parameters after creating a server (scaling). </br>
Microsof has several tools that you can use to provision services, such as: </br>
  1. Microsoft Azure Portal: Most convenient way to provision a service. </br>
  2. Azure CLI (Command-Line Interface): Set of commands that the user can run from the OS (Operating System) prompt or the Cloud Shell. The user can create and manage these commands to create and manage Azure resources. </br>  
  3. Azure PowerShell: Familiar to administrators, create and manage Azure resources. </br>
  4. Azure Resource Manager templates: Describes the services that you want to deploy in a text file. Format known is .JSON, so you can define infrastructure and configuration for your project. </br>

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
Normally it falls in two cases:
1. Semi-structured: Data that contains fields, they don't have to be the same every entity. They must be formatted in such a way that an application can parse and process it. Normally they are storage as [JSON](https://learn.microsoft.com/en-us/sql/relational-databases/json/json-data-sql-server?view=sql-server-ver16) documents.
It has several programs that we can used to "break up" this document from JSON format, extracting individual data: </br>
1.1. Avro by Apache: storage data as binary </br>
1.2. ORC by HortonWorks: Organizes data into columns rather than rows. </br>
1.3. Parquet by Cloudera & Twitter: Contains row groups, each row group contains one or more chunks of data

2. Non-structured: Unstructured data doesn't naturally contain fields. For example files like Audio, Video, Images and Media Streams. you have to storage them in a special program for this files. Such as Azure Blob Storage.

In cases that we cannot know which structure of the data in advance, we can consider it as non-relational data. Where for example, the customer can have several telephone numbers as thei addresses. So in these cases, we want to save the data the fastest way as possible and we will not storage it in a relational structure now, appropriete is just to storage de data, and then process lately.
The entity are usually storage in Key-Value (as ID field, for example).
More advanced non-relational systems support indexing. 
[Azure Cosmos DB](https://learn.microsoft.com/en-us/azure/cosmos-db/index-overview) is a non-relational system support this indexing.
Cases we can use Non-relational databases: 
1. IoT & telematics:
   - Ingest large amounts of data
   - Quick storage utilized by analytics services
   - Real-time data processing
2. Retail & marketing:
   - CosmosDB for Windows Store and Xbox Live
   - Used in the retail industry for storage and process pipelines
3. Gaming:
   - Databawse tier crucial
   - Cloud delivers customized and personalized user content
   - Low latency for speedy & greater user experience
   - Capability to handle new game launches and feature updates
4. Web & mobile
   - Azure Cosmos DB commonly used
   - Well suited for modern requirements to deliver rich user experiences
   - Cosmos DB SDKs for iOS and Android apps via Xamarin





### Types of non-relational and NoSQL data
When reading non-relational databases, it's normal to hear about NoSQL. it's available on Azure services as Cosmos DB.
key-value store: inserting and querying data. Key identify the data, and the value holds the data for the item. 

### Recommend the correct data store
### When to use non-relational data
  
## 3.2 Non-relational data offering on Azure
### Identify Azure data services for non-relational workloads
### Azure Cosmos DB APIs
Globally distributed database that supports NoSQL options

### Azure Table storage
A NoSQL store that hosts unstructured data independent of any schema

### Azure Blob storage
Storage service for very large objects, such as video files or bitmaps/ (Blob = Binary Large Object)

### Azure File storage
File shares that can be accessed and managed like a file server

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




