---
layout: post
title: Databases
---
 


A **database** is a collection of information that is organized so that it can easily be accessed, managed, and updated. Any modern database is created and managed by a Database Management System (DBMS).


In computing, databases are sometimes classified according to their organizational approach. The most prevalent approach is the relational database, a tabular database in which data is defined so that it can be reorganized and accessed in a number of different ways. A distributed database is one that can be dispersed or replicated among different points in a network.


Computer databases typically contain aggregations of data records or files, such as sales transactions, product catalogs and inventories, and customer profiles. 


Typically, a database administration involves providing users with the capabilities of read/write access, specifying report generation, and analyzing usage of the database.


Moi university’s databases are developed and maintained by ICT staff as per request from the user departments and as need arises. The following are among the databases in Moi University;


* Finance management information system 
- Students hostel online booking system(MUHMS)
+ Moi university students clearance system(SOCS)
* Personnel system database
- E-Learning database
+Mail database


Each of the above databases has a distributed server which can be accessed within the domain of the Moi University Wide Area Network. All the servers for the above databases are housed within the server room, and the overall database infrastructure is monitored and managed by the database administrator, who ensures there is constant and consistent access to the information therein in the databases by the relevant clients.


Network monitoring and management involves checking for the following parameters:


* Availability
- Reliability
+ Performance


Components of a network that is monitored can either be systems or services
Systems include: Routers, Switches and servers and monitored services include: HTTP, DNS, SMTP and SMNP.


## Database Backup Techniques

In database administration we also dealt with database back up techniques and methods; with reference to MySQL databases.


Backup is the activity of copying files or databases so that they will be preserved in case of equipment failure or other catastrophe. Backup is usually a routine part of the operation of large businesses with mainframes as well as the administrators of smaller business computers.


Some of the techniques used to make MySQL database backups are as outlined below:


### 1. Making a Hot Backup with MySQL Enterprise Backup


MySQL Enterprise Backup product is used to do physical backups of entire instances or selected databases, tables, or both. This product includes features for incremental and compressed backups. Backing up the physical database files makes restore much faster than logical techniques such as the mysqldump command.


### 2. Making Backups by Copying Table Files


For storage engines that represent each table using its own files, tables can be backed up by copying those files. For example, MyISAM tables are stored as files, so it is easy to do a backup by copying files (*.frm, *.MYD, and *.MYI files).


### 3. Making Incremental Backups by Enabling the Binary Log
MySQL supports incremental backups: You must start the server with the - -log-bin option to enable binary logging. The binary log files provide you with the information you need to replicate changes to the database that are made subsequent to the point at which you performed a backup. At the moment you want to make an incremental backup (containing all changes that happened since the last full or incremental backup), you should rotate the binary log by using flush logs. This done, you need to copy to the backup location all binary logs which range from the one of the moment of the last full or incremental backup to the last but one. These binary logs are the incremental backup; at restore time.


### 4. Making Backups Using Replication Slaves
If you have performance problems with your master server while making backups, one strategy that can help is to set up replication and perform backups on the slave rather than on the master.
 If you are backing up a slave replication server, you should back up its master.info and relay-log.info files when you back up the slave's databases, regardless of the backup method you choose. These information files are always needed to resume replication after you restore the slave's data.
