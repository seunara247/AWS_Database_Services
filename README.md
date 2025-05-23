# AWS Database Services Project

This project demonstrates the use of **AWS RDS (MySQL)** and **AWS DynamoDB** by launching an RDS instance, performing basic SQL operations, setting up a key-value store in DynamoDB, and understanding the key differences between the two AWS database services.

## Overview

### AWS RDS (MySQL)

Amazon RDS (Relational Database Service) is a fully managed database service that supports engines like **MySQL**, **PostgreSQL**, **MariaDB**, and others. It is ideal for applications that need structured data with relationships, SQL queries, and transaction support.

##### Use Cases:

- E-commerce applications  

- Inventory management  

- Financial transactions  

##### Benefits:

- Automates backups, patching, and maintenance  

- Supports secure access using **VPC**, **IAM**, and **Security Groups**


### AWS DynamoDB

DynamoDB is a serverless NoSQL database service for key-value and document-based data. It offers high availability, durability, and millisecond latency.

##### Use Cases:

- Applications that need low-latency, high-throughput access to key-value or JSON-like data

##### Benefits:

- Fully serverless

- Auto-scaling and highly available

- Built-in security and multi-region replication

### Comparison: RDS vs DynamoDB

- **Database Type**: AWS RDS(MySQL) is Relational (SQL) while AWS DynamoDB is NoSQL (Key-Value / Document)

- **Schema**: AWS RDS uses Fixed schema (structured rables, columns, types) while AWS DynamoDB uses Flexible schema                  

- **Query Language**: AWS RDS uses SQL as it's query language while AWS DynamoDB uses DynamoDB API with no SQL

- **Relationships**: AWS RDS supports joins, foreign keys while AWS DynamoDB has no native support for joins, flat data              

- **Scalability**: AWS RDS uses Vertical scaling (instance size) while AWS DynamoDB uses Horizontal scaling (auto-scaling, partitions) 

- **Latency**: AWS RDS has higher latency while AWS DynamoDB has Low latency                      

- **Management**: AWS RDS is more manual configuration while AWS DynamoDB is fully managed and serverless     

### Prerequisites

- AWS account

- MySQL GUI client (e.g., **MySQL Workbench**)

- AWS CLI (optional for DynamoDB CLI actions)

### RDS (MySQL) Setup

**Instance Configuration:**

- Region: `af-south-1` (or your preferred region)

- Engine: `MySQL`

- Instance Type: `db.t3.micro` (Free Tier eligible)

- Storage: `20 GB`

- Public access: Enabled

- Ensure **DNS resolution** is enabled in VPC settings

**Connect to RDS using MySQL Workbench:**

- **Hostname:** your-RDS-endpoint.rds.amazonaws.com  

- **Port:** 3306  

- **Username:** your-username  

- **Password:** your-password  

### Screenshots:

- RDS instance setup

- MySQL Workbench connection

- SQL query execution

##DynamoDB Setup

- Table Name: MydynamoDB

- Primary Key: UserID (String)

- Sample Items:Testing:

- Add, edit, and delete items using the DynamoDB console

- Query using the UserID key

- View table structure and item details

### Screenshots:

- Table creation

- Item insertion and query results

###Conclusion

This project helped me understand the difference between relational (SQL) and NoSQL database models on AWS. I practiced how to:

- Launch and connect to an RDS MySQL instance

- Write and run SQL queries

- Create and use a DynamoDB key-value store

- Compare management, performance, and structure between RDS and DynamoD
