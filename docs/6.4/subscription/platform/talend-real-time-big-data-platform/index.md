---
title: "Talend Real-time Big Data Platform"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

# Introduction

Talend Real-time Big Data Platform includes all the features in Big Data Platform, including:
- Add Spark Streaming
- ESB optional but generally required to load messages into message brokers

Built on top of Talend's data integration solution, the big data solution is a powerful tool that enables users to access, transform, move and synchronize big data by leveraging the Apache Hadoop Big Data Platform and makes the Hadoop platform ever so easy to use.

Talend's ESB solution provides a versatile and flexible, enterprise service bus (ESB) that allows organizations to address any integration challenge - from simple departmental projects to complex, heterogeneous IT environments.

In the field of data quality, users can profile and cleanse the data available in different data sources, browse the analyzed data and generate reports on analysis results from Talend DQ Portal.

# Architecture

Talend Real-time Big Data Platform architecture is similar to [Big Data Platform architecture][big-data-platform-reference-architecture] with additional optional ESB Product features.

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

For Physical Reference Architecture and Sizing details please refer to [Big Data Architecture][big-data-platform-reference-architecture] and combine it with [ESB Reference Archtitecture][esb-reference-architecture] (if required)


<!-- links -->

[logical-architecture-details]: https://help.talend.com/reader/5DJN_N7G494oW~IzuXEhGQ/ofvHcWVPeSfgg3sYiLZ4qw "Talend Real-time Big Data Platform functional architecture"

[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/cNrWgOPncdn8vxSL3iMOVw/content "Talend Real-time Big Data Platform functional architecture Picture"

[big-data-platform-reference-architecture]: ./../talend-big-data-platform/index.md

[esb-reference-architecture]: ./../../entry/talend-esb/index.md
