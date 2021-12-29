# WB3Tech SQL Database Operator Specifications
## Overview

The SQL Database Operator codifies Day 2 management & operations.  These operations currently include:

 - Updating the database DDL

The SQL database being managed does not need to reside within the same kubernetes cluster, or even on a kubernetes cluster.  It was designed to provide a way to autnonoize operations of any SQL database, regardless of the technology that hosts the database instance. 

### Supported Database Technologies
- PostgreSQL

### Assupmtions
The operator assumes the following:

 - A network accessible instance of a SQL database is accessible to the operator.
 - The *Adminstrator Credentials* have the proper authority to execute all functions in the SQL DDL resource.

### Limitations
The follow aspects are limtations of the operator:

 - The management and operations actions are scoped to capbilties provided by the binary APIs utilized for the oeprator.
 - It does not provide any complinace or security hardening features.


### Specifiations
This section defines the specifictions, protocol, and standards codified into the operator.

#### The DDL Protocol
The operator embodies a very specific protocol for handling the ddl updates.

#### Diagrams

##### UML

###### State
 - SQL Databse Operator State Diagram

###### Sequence
 - Update DDL Sequence