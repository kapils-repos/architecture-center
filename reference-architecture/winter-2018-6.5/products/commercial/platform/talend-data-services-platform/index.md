---
title: "Talend Data Services Platform"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.5"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---
# Talend Data Services Platform

## Introduction

Talend Data Services Platform combines Talend products into a common set of powerful, easy-to-use solutions.

-  Talend's data integration solution helps companies deal with growing system complexities by addressing both ETL for analytics and ETL for operational integration needs and offering industrialization features and extended monitoring capabilities.

- Talend's ESB solution provides a versatile and flexible, enterprise service bus (ESB) that allows organizations to address any integration challenge - from simple departmental projects to complex, heterogeneous IT environments.

- In the field of data quality, users can profile and cleanse the data available in different data sources, browse the analyzed data and generate reports on analysis results from Talend DQ Portal.

## Architecture

Talend Data Services Platform leverages Talend Data Integration & Talend ESB by being built on top of them. It is a bundle of Data Integration, ESB and Data Quality features.

The Logical Architecture give us a high level view of various components that make up the platform and Physical Architecuture provides guidelines for various deployment environments.

## Logical Reference Architecture

The Talend Data Services Platform functional architecture is an architectural model that identifies Talend Data Services Platform functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks. For more details on the individual components of Logical Architecture please refer <a href="https://help.talend.com/reader/zdwY1pAmGxrugwm~piPJuQ/SHGZkrdI2BSfSp~BsLFxZQ" target="_blank">Talend Help documentation</a>.
The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]


## Physical Reference Architecture & Recommended Sizing

The physical architecture and recommended sizing is similar to that of [Talend ESB][esb-reference-architecture] along with optional Data Quality Components installed.

<!-- links -->
[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/x2DFpubxTuV32IyyKhTNyw/content "Talend Data Services Platform functional architecture"
{:.img-fluid}
[esb-reference-architecture]: ./../../entry/talend-esb/index
