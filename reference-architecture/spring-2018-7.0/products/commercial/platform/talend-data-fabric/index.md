---
title: "Talend Data Fabric"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---
# Talend Data Fabric

## Introduction

Talend Data Fabric combines Talend products into a common set of powerful, easy-to-use solutions.

- **Talend's data integration** solution helps companies deal with growing system complexities by addressing both ETL for analytics and ETL for operational integration needs and offering industrialization features and extended monitoring capabilities.

- Built on top of Talend's data integration solution, the **big data solution** is a powerful tool that enables users to access, transform, move and synchronize big data by leveraging the Apache Hadoop Big Data Platform and makes the Hadoop platform ever so easy to use.

- **Talend's ESB solution** provides a versatile and flexible, enterprise service bus (ESB) that allows organizations to address any integration challenge - from simple departmental projects to complex, heterogeneous IT environments.

- The **MDM solution** unifies any amount of data - from customers to products to suppliers and beyond - into a single and actionable “version of the truth.” It combines real-time data, applications, and process integration with embedded data governance and stewardship to share across on-premises, cloud and mobile applications.

- In the field of data quality, users can profile and cleanse the data available in different data sources, browse the analyzed data and generate reports on analysis results from Talend DQ Portal.

## Architecture

Talend Data Management Platform leverages Talend Data Integration, ESB , MDM and Data Quality by being built on top of them.

The Logical Architecture give us a high level view of various components that make up the platform and Physical Architecuture provides guidelines for various deployment environments.

## Logical Reference Architecture

The Talend Data Fabric functional architecture is an architectural model that identifies Talend Data Fabric functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks. For more details on the individual components of Logical Architecture please refer <a href="https://help.talend.com/reader/NGFVbCXsCwp_DpVt~CLweQ/NOrVLeirkJts53uPPR1ZQQ" target="_blank">Talend Help documentation</a>.

The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]

## Physical Reference Architecture

Please refer to reference architecture of below solutions for getting the information on physical architecture and recommended sizing guidelines.

- **[Data Management Reference Architecture][dm-reference-architecture]**

- **[ESB Reference Architecture][esb-reference-architecture]**

- **[MDM Reference Architecture][mdm-reference-architecture]**

- **[Big Data Reference Architecture][big-data-reference-architecture]**


<!-- links -->
[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/5IEBjcHsD9le1xEylXhE8A/content "Talend Data Fabric"
{:.img-fluid}
[dm-reference-architecture]: ./../talend-data-management-platform/index
[esb-reference-architecture]: ./../../entry/talend-esb/index
[mdm-reference-architecture]: ./../talend-mdm-platform/index
[big-data-reference-architecture]: ./../../entry/talend-big-data/index