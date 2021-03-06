---
title: "Talend ESB"
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

Talend ESB is a reliable and scalable enterprise service bus (ESB) that lets development teams manage integration projects in a holistic manner, combining integration of applications and data management in complex and heterogeneous computing environments. This page describes the various components that make up the Talend ESB Platform, Logical Architecture, Physical Architecture & Sizing guidelines. 

# Architecture

Talend Data Management Platform leverages Talend Data Integration by being built on top of DI Reference Architecture. It is a bundle of Data Integration and Data Quality features.

Key Features:
- **[ESB Data Services][esb-services]**
- **[ESB Mediation Routes][esb-routes]**
- **[Talend ESB Runtime][esb-runtime]**

 The Logical Architecture give us a high level view of various components that make up the platform and Physical Architecuture provides guidelines for various deployment environments.

## Talend Platform

## Logical Reference Architecture

The Talend ESB functional architecture is an architectural model that identifies Talend ESB functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks.

The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]

For more details on the individual components of Logical Architecture please refer [Talend Help documentation][logical-architecture-details]. 

## Physical Reference Architecture

### Guiding Principles (Same as for Data Integration):
- We will have 4 environments as per our best practices
- SDLC with CI is optional but recommended addon
- DR environment is an addon depending on customer requirements

### Environments:

- **[Development Environment][esb-dev]**

- **[Testing Environment][esb-test]**

- **[Pre-Prod & Production Environment][esb-prod]**



## Recommnded Sizing

Workstation/Server Role|OS|CPU|RAM|SSD Disk Size
--- | --- | --- | --- | ---
Client PC|Windows/Linux/Mac|4 Cores i7 Processor or equivalent|16 GB|500 GB
Talend Administration Center|Windows/Linux|4 Cores |8 GB RAM Minimum, 32 GB Recommended for 1000s of Jobs|300GB+ Minimum (for software & logs)
IAM Server|Windows/Linux|4 Cores Minimum,8+ Cores Recommended|16 GB RAM Recommended|300+ GB
ESB Server|Windows/Linux|4 Cores Minimum,8+ Cores Recommended|16 GB RAM Recommended|300+ GB
Centralized Log Server|Windows/Linux|4 Cores Minimum|16 GB RAM|300+ GB
Shared Nexus Server|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|300+ GB
Git Server (Better in Saas Mode)|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|50+ GB
CI Server|Windows/Linux|4 Cores Minimum,8 Cores Recommended|16 GB RAM|300+ GB


<!-- links -->

[logical-architecture-details]: https://help.talend.com/reader/6waQVOIx1A61D8607u5qfw/n6SuKCQs40etXM8HnisZLQ "Functional architecture of Talend ESB"
[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/EGGe3ssElK_mb6HCWxIukQ/content "Functional architecture of Talend ESB"

[esb-services]: ./esb-data-services.md
[esb-routes]: ./esb-routes.md 
[esb-runtime]: ./esb-runtime.md 

[esb-dev]: ./esb-physical-reference-architecture-dev.md
[esb-test]: ./esb-physical-reference-architecture-test.md 
[esb-prod]: ./esb-physical-reference-architecture-prod.md 

