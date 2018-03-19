---
title: "Talend Big Data Platform"
creationDate: "02/27/2018"
modifiedDate: "02/28/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

# Introduction

Built on top of Talend's data integration solution, the big data solution is a powerful tool that enables users to access, transform, move and synchronize big data by leveraging the Apache Hadoop Big Data Platform and makes the Hadoop platform ever so easy to use.

Big Data Platform includes all the features in Data Management Platform, including:
- Data Quality Components in the Studio
- Data Quality for Big Data Components in the Studio
- Profiling Perspective in Studio
- Talend Data Quality Portal
- HA Support for Job Conductor in TAC
- Virtual Servers for Job Load Balancing in TAC
- Talend Data Mapper
- SAP RFC Server

# Architecture

Big Data Platform architecture is similar to [Data Integration architecture][big-data-reference-architecture].

## Talend Platform


## Logical Reference Architecture

The Talend Big Data Platform functional architecture is an architectural model that identifies Talend Big Data Platform functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks.

The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]

### Highlights (Same as for Data Integration & in-addition below):
- JobServers should be setup for plain DI ETL Jobs and for Big Data Jobs.
- There should be a separation of concern.
- While the Logical Reference Architecture diagram shows JobServer outside the cluster, we recommend, as a best practice, to install the - JobServer on the Edge nodes of a cluster.

For more details on the individual components of Logical Architecture please refer [Talend Help documentation][logical-architecture-details].

For Physical Reference Architecture and Sizing details please refer to [Big Data Architecture][big-data-reference-architecture]


<!-- links -->

[logical-architecture-details]: https://help.talend.com/reader/ZRnt3jPkO_6Os2rl1NpJrQ/5O2~FCcsS~5HP_NEh6SzpQ "Talend Big Data Platform functional architecture"

[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/gv2tNatPYtPp~7P6oYddrQ/content "Talend Big Data Platform functional architecture Picture"

[big-data-reference-architecture]: ./../../entry/talend-big-data/index.md
 
