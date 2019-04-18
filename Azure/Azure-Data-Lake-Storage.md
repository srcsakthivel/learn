## What is ADLS?
- Azure Data Lake Storage.
- A data lake is a repository of data that is stored in its natural format, usually as blobs or files.
- it is a comprehensive, scalable and cost-effective solution

## Offers:
- combines a file system with a storage platform
- builds on Azure Blob storage capabilities to optimize it specifically for analytics workloads
- integration enables 
  - analytics performance
  - the tiering and data lifecycle management capabilities of Blob storage
  - the high-availability, security, and durability capabilities of Azure Storage
  
## Benefits:
- can deal with variety and volume of data at exabyte scale while securely handling hundreds of gigabytes of throughput
- you can use Data Lake Storage Gen2 as the basis for both real-time and batch solutions
- **Hadoop Distributed File System - HDFS**, access it through compute technologies including Azure Databricks, Azure HDInsight, and Azure SQL Data Warehouse without moving the data between environments
- **Security**
  - Data Lake Storage Gen2 supports access control lists (ACLs) and Portable Operating System Interface (POSIX) permissions, 
  - Set permissions at a directory level or file level for the data stored
  - Security is configurable through technologies such as Hive and Spark, or utilities such as Azure Storage Explorer
  - Data that is stored is encrypted at rest by using either Microsoft or customer-managed keys
- **Performance**
  - Organizes the stored data into a hierarchy of directories and subdirectories, much like a file system, for easier navigation
  - Data processing requires less computational resources, reducing both the time and cost.
- **Data redundancy**
  - LRS - data redundancy in a single data center with locally redundant storage
  - GRS - a secondary region by using the Geo-redundant storage
