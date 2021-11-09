# Databases
Web applications utilize back end databases to store various contents and information related to the web application

## Relational SQL
Relational SQL databases store their data in tables, rows and columns. Each table can have unique key which can link tables together and create relationships between tables.

![[Pasted image 20211109003952.png]]

> The relationship between tables within databases is called Schema.

Some of the most common rational databases :

||
--|--
**Type** | **Description**
**MySQL** | The most commonly used databases around the internet. It is an opensource databases and can be used completely free of charge.
**MSSQL** |  Microsoft's implementation of a rational database. Widely used with windows servers and IIS web servers.
**Oracle** | A very reliable databases for big businesses, and is frequently update with innovative database solution make it faster and are more reliable. It can be costly, even for big businesses.
**PostgreSQL** | Another free and open-source rational database. It is designed to be easily extensible, enabling adding advanced new features without needing a major change to the initial database design.

 Other common  database include : **SQL lite, MariaDB, Amazon Aurora and Azure SQL.**
 
 ## Non-Relation (NoSQL)
 A non-rational database does not use tables, rows, columns, primary keys, relationships, or schemas. Instead, a NoSQL database stores data using various storage models depending on the type of data stored.
 
 Due to lack of a defined structure of the databases NoSQL  databases are very scalable and flexible. 
 When dealing with datasets that are not very well defined and structured, a NoSQL database would be the best choices for storing our data.
 
 There are 4 common storage models for NoSQL databases :
 
 - Key-value 
 - Document-based 
 - Wide-Column
 - Graph

Each of above models has a different way of storing data. For example, the **key-value** model usually stores data in **JSON** or **XML**, and has a key for each pair, storing all of its data as its value:

![[Pasted image 20211109184836.png]]
 
![[Pasted image 20211109184941.png]]

The **Document-Based** model store data in complex **JSON** objects and each object has certain meta-data while storing the rest of the rest similar to the **key-value** model.

Some of the most common **NoSQL** database included :

||
--|--
**Type** | **Description**
**MongoDB** | The most common NoSQL database. It is free and open-source uses the **Document-Based** model and stores data in **JSON** objects.
**ElasticSearch** | Free and Open-source It is optimized for storing and analyzing huge datasets. Searching for data within this database is very fast and efficient.
**Apache Cassandra** | Free and Open-Source. It is very scalable and optimized for gracefully handling faulty values.

Other common **NOSQL** database include : **Redis , Neo4j, CouchDB and Amazon DynamoDB



