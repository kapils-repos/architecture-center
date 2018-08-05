---
title: "Talend Big Data"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

# Talend Big Data

## Introduction

Built on top of Talend's data integration solution, the big data solution is a powerful tool that enables users to access, transform, move and synchronize big data by leveraging the Apache Hadoop Big Data Platform and makes the Hadoop platform ever so easy to use.

## Architecture

Big Data architecture is similar to [Data Integration architecture][di-arch].

## Logical Reference Architecture

The Talend Big Data functional architecture is an architectural model that identifies Talend Big Data functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks. For more details on the individual components of Logical Architecture please refer <a href="https://help.talend.com/reader/jQt1t9p~sZh3MMJ8TxPc~w/mDNqOPohoBU11tZ~Lw1ODw" target="_blank">Talend Help documentation</a>

The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]


### Highlights (Same as for Data Integration & in-addition below):
- JobServers should be setup for plain DI ETL Jobs and for Big Data Jobs.
- There should be a separation of concern.
- While the Logical Reference Architecture diagram shows JobServer outside the cluster, we recommend, as a best practice, to install the - JobServer on the Edge nodes of a cluster.

## Physical Reference Architecture

### Edge Node or Gateway Node
- Has all the necessary libraries and client components present
- Has the current configuration of the cluster
- Do not mix with actual cluster service nodes
- Trusted by the cluster to have end users running CLI based tools like beeline, hdfs, hive, tools, etc.
- You will require as many Edge Nodes as required to meet your solution requirements.

### Recommendations
- Job Server for Big Data Jobs should be installed on Cluster Edge Nodes
- Job Server on Edge Nodes should be running Linux OS
- Linux OS will allow impersonation
- Use Job Server outside the cluster for pure DI batch jobs for separation of concerns


### Environments

- **[Development Environment][bd-dev]**

- **[Testing Environment][bd-test]**

- **[Pre-Prod & Production Environment][bd-prod]**


## Recommended Sizing

Workstation/Server Role|OS|CPU|RAM|SSD Disk Size
--- | --- | --- | --- | ---
Client PC|Windows/Linux/Mac|4 Cores i7 Processor or equivalent|16 GB|500 GB
Talend Administration Center|Windows/Linux|4 Cores |8 GB RAM Minimum, 32 GB Recommended for 1000s of Jobs|300GB+ Minimum (for software & logs)
Job Server(s)|Windows/Linux|4 Cores Minimum,8+ Cores Recommended|16 GB RAM Minimum,128 GB Recommended|300+ GB
Edge Node(s)|Linux|4 Cores Minimum,32+ Cores Recommended|16 GB RAM Minimum,256 GB Recommended|1+ TB
Centralized Log Server|Windows/Linux|4 Cores Minimum|16 GB RAM|300+ GB
Data Prep & Data Stewardship Server|Windows/Linux|4 Cores Minimum|32 GB RAM|300+ GB
Shared Nexus Server|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|300+ GB
Git Server (Better in Saas Mode)|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|50+ GB
CI Server|Windows/Linux|4 Cores Minimum,8 Cores Recommended|16 GB RAM|300+ GB


<!-- links -->
[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/KDRCD9_GS1jajiyEG0Dt0w/content "Talend Big Data functional architecture Picture"
{:.img-fluid}
[di-arch]: ./../talend-data-integration/index
[bd-dev]: ./bigdata-physical-reference-architecture-dev
[bd-test]: ./bigdata-physical-reference-architecture-test
[bd-prod]: ./bigdata-physical-reference-architecture-prod
