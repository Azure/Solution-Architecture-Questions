# Migration or Green Field Implementation

* Is this an application being migrated to Azure from somewhere or is it a green field implementation ?

<br/>

<br/>

# Database Migration

* What databases are being used - and what versions ?
* Is this coming from another cloud platform or on-premise ?
* What are the challenges you are facing today that should be addressed as part of the migration ?
* What is the current size of the database ?
* How much outage is acceptable whem migrating the database to Azure ?

<br/>

<br/>


# Green field implementation

* Do you need guidance on what type of database to use ?
* What is going to be the initial size of the database ?

<br/>

<br/>

# Generic Questions

* Which database technologiess are used ? 
* What is the initial size of each database ?
* How much the database grows in size in a year ?
* Is there any ETL or ELT out of this database  ?  

     _If yes_ - What is the target of this ETL/ELT - another database / data lake / storage ?

     _If no_  - What is the strategy to archive / delete old data from the database ?

* What is the RTO and RPO for the database ?
* What is the BCDR ( Business continuity and Disaster Revovery ) strategy of the applicatoin and the database ?
* What is the maximum number of user sessions that will be active on the database ?
* Do you have any specific need for database scale up / down ?
* Is the database going to be accessed from any specific network / Vnet or Private network ?
* What database drivers would you use to connect to it ?
* Do you use database triggers and stored procedures ?
* What is the peak IOPS required out of the database ?
* Read / Write ratio ?

<br/>

<br/>

# CosmosDB Questions

* Do you have experence with design of NoSQL databases ?
* Which API you are going to use ?
* Do you need multi-region write ?

<br/>

<br/>

# MySQL Questions

* What version of MySQL ?
* MySQL storage engine used ?

<br/>

<br/>

# Postgres Questions

* What version of Postgres ?
* Which extensions are being used today ?

<br/>

<br/>

# Redis Questions

* What versions of Redis ?
* Which modules are being used today ? 

<br/>

<br/>

# SQL Questions

* What version of SQL is being used today ?
* Do you use any feature in the database that needs access to underlying OS ?
* Do you run cross database query or filestream or extended stored procedure ?

<br/>

<br/>

## Resources

* Feature Diifference Between [Azure SQL DB and SQLMI](https://docs.microsoft.com/en-us/azure/azure-sql/database/features-comparison)

<br/>

<br/>

## Tools