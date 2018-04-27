---
title: "Talend Data Integration"
creationDate: "02/27/2018"
modifiedDate: "04/26/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDate: "02/27/2018"
latest.revision: 2
author: "Lokesh"
---

# Introduction

Talend's data integration solution helps companies deal with growing system complexities by addressing both ETL for analytics and ETL for operational integration needs and offering industrialization of features and extended monitoring capabilities. This page describes the various components that make up the Talend Platform, Logical Architecture, Physical Architecture , Best Practices & Guidelines based on our current support and guidelines. 

# Architecture

The Talend Data Integration Product consists of Platform Components which are designed & integrated to provide the ETL functionality needed for serving many business requirements. The Logical Architecture give us a high level view of various components that make up the platform and Physical Architecuture provides guidelines for various deployment environments.

## Talend Platform

### Oracle Java JDK – a Talend Pre-requisite
Server side and client side components all require an Oracle JDK (Java Development Kit) to run. Each component has its own specific pre-requisites, but the need for a JDK is consistent across all Talend components.

- As of Talend v6 only JDK 8 is supported by Talend* – Oracle no longer supports Java 7
  Exception: IBM AIX only has IBM Java 7 support, but only for specific Talend server components
- Talend recommends that you use the same JDK version on all clients and servers
- Compatible platforms / Java versions can be found in the [product documentation][product documentation]


The components that make up Talend Data Integration (and thus support the requirements of Kimball’s ETL Subsystems) are:

- **[Talend Studio][Talend Studio]**

- **[Talend Metadata Bridge][Talend Metadata Bridge]**

- **[Talend SAP RFC Server][Talend SAP RFC Server]**

- **[Talend Administration Center][Talend Administration Center]**

- **[Metadata Repository: Subversion or GIT][Metadata Repository]**

- **[Artifact Repository][Artifact Repository]**

- **[CommandLine][CommandLine]**

- **[JobServer][JobServer]**

- **[Talend CI Builder][Talend CI Builder]**

- **[Talend Activity Monitoring Console][Talend Activity Monitoring Console]**

- **[Talend Log Server][Talend Log Server]**

## Logical Reference Architecture

The Talend Data Integration functional architecture is an architectural model that identifies Talend Data Integration functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks.
The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]

For more details on the individual components of Logical Architecture please refer [Talend Help documentation][logical-architecture-details]. 

## Physical Reference Architecture

### Guiding Principles:
- We will have 4 environments as per our best practices
- SDLC with CI is optional but recommended addon
- DR environment is an addon depending on customer requirements
- Data Prep and Data Stewardship are optional components.

### Environments:

- **[Development Environment][di-dev]**

- **[QA, UAT & Production Environment][di-prod]**

- **[Deployment Strategy][deployment]**


## Recommnded Sizing

Workstation/Server Role|OS|CPU|RAM|SSD Disk Size
--- | --- | --- | --- | ---
Client PC|Windows/Linux/Mac|4 Cores i7 Processor or equivalent|16 GB|500 GB
Talend Administration Center|Windows/Linux|4 Cores |8 GB RAM Minimum, 32 GB Recommended for 1000s of Jobs|300GB+ Minimum (for software & logs)
Job Server(s)|Windows/Linux|4 Cores Minimum,8+ Cores Recommended|16 GB RAM Minimum,128 GB Recommended|300+ GB
Centralized Log Server|Windows/Linux|4 Cores Minimum|16 GB RAM|300+ GB
Data Prep & Data Stewardship Server|Linux|4 Cores Minimum|32 GB RAM|300+ GB
Shared Nexus Server|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|300+ GB
Git Server (Better in Saas Mode)|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|50+ GB
CI Server|Windows/Linux|4 Cores Minimum,8 Cores Recommended|16 GB RAM|300+ GB


<!-- links -->
[product documentation]: https://help.talend.com/reader/RexlZLQDFJ5kZX15Y4ZebQ/WwuniyNr4hf4hn62WSyQww "Talend Data Integration Installation Guide for Windows"
[logical-architecture-details]: https://help.talend.com/reader/nXPtKhielAtSqFD6_f7~OQ/WwuniyNr4hf4hn62WSyQww "Talend Data Integration Logical Architecture"
[Java]: ./../../../talend-components/java.md
[Talend Studio]: ./../../../talend-components/talend-studio.md
[Talend Metadata Bridge]: ./../../../talend-components/talend-metadata-bridge.md
[Talend SAP RFC Server]: ./../../../talend-components/talend-sap-rfc-server.md

[Talend Administration Center]: ./../../../talend-components/talend-administration-center.md
[Artifact Repository]: ./../../../talend-components/artifact-repository.md
[CommandLine]: ./../../../talend-components/command-line.md
[Metadata Repository]: ./../../../talend-components/metadata-repository.md
[JobServer]: ./../../../talend-components/job-server.md
[Talend CI Builder]: ./../../../talend-components/talend-ci-builder.md

[Talend Activity Monitoring Console]: ./../../../talend-components/talend-activity-monitoring-console.md
[Talend Log Server]: ./../../../talend-components/talend-log-server.md

[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/cdDHY~srerWZK4ptDezsiA/content "Talend Data Integration Installation Guide for Windows"

[di-dev]: ./di-physical-architecture-dev.md
[di-prod]: ./di-physical-architecture-prod.md 
[deployment]: ./di-deployment-strategy.md
