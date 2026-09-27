 Azure Database Resilience & Secure Connectivity

📌 Project Overview

This project implements a **secure and highly available Azure SQL database architecture** using Microsoft Azure services.

The solution protects database connectivity and provides **cross-region disaster recovery** using Azure SQL Failover Groups.

 🏗️ Architecture

Primary SQL Server:** Central India
Secondary SQL Server:** Korea Central
Azure SQL Database:** `EcommerceDB`
Azure SQL Failover Group:** `ecommerce-fog`
Virtual Networks:** Primary and Secondary VNets
Private Endpoints:** Secure private database connectivity
Private DNS:** Resolves database endpoints privately
Public Network Access:** Disabled

 🔐 Security

Private Endpoints allow database access through the Azure Virtual Network instead of the public internet. Public network access is disabled to improve security.

 🔄 High Availability & Disaster Recovery

The primary database is replicated to the secondary region using an **Azure SQL Failover Group**. This provides regional redundancy and enables failover during a regional outage.

 ☁️ Azure Services Used

* Azure SQL Database
* Azure SQL Server
* Azure Virtual Network
* Azure Private Endpoint
* Azure Private DNS
* Azure SQL Failover Group
* Azure Resource Manager

 📁 Infrastructure as Code

The Azure environment can be exported as **ARM/Bicep/Terraform templates** and stored in GitHub for version control and reproducible deployment.

 🎯 Outcome

The project provides a **secure, highly available, and disaster-resilient e-commerce database architecture** with private connectivity and cross-region redundancy.
