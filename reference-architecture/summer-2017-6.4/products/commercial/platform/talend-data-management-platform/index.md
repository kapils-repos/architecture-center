---
title: "Talend Data Management Platform"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---
# Talend Data Management Platform

## Introduction

Talend Data Management Platform combines Talend products into a common set of powerful, easy-to-use solutions. This page describes the various components that make up the Talend Platform, Logical Architecture, Physical Architecture & Sizing guidelines.

## Architecture

Talend Data Management Platform leverages Talend Data Integration by being built on top of DI Reference Architecture. It is a bundle of Data Integration and Data Quality features.

### Key Features
- Data Quality Components in the Studio
- Profiling Perspective in Studio
- Talend Data Quality Portal
- HA Support for Job Conductor in TAC
- Virtual Servers for Job Load Balancing in TAC
- Talend Data Mapper
- SAP RFC Server

The Logical Architecture give us a high level view of various components that make up the platform and Physical Architecuture provides guidelines for various deployment environments.

## Logical Reference Architecture

The Talend Data Management Platform functional architecture is an architectural model that identifies Talend Data Management Platform functions, interactions and corresponding IT needs. The overall architecture has been described by isolating specific functionalities in functional blocks. For more details on the individual components of Logical Architecture please refer <a href="https://help.talend.com/reader/ZASi1iqSzd1Hv0sG_S_xtg/uOde2CK5Gjj_DIH_fy458A" target="_blank">Talend Help documentation</a>.

The following chart illustrates the main architectural functional blocks.

![alt text][Logical Architecture]




## Physical Reference Architecture

### Guiding Principles (Same as for Data Integration)
- We will have 4 environments as per our best practices
- SDLC with CI is optional but recommended addon
- DR environment is an addon depending on customer requirements
- Data Prep and Data Stewardship are only going to be installed if customer wants them on-premise.

### Environments

- **[Development Environment][dm-dev]**

- **[Testing Environment][dm-test]**

- **[Pre-Prod & Production Environment][dm-prod]**

- **[Deployment Strategy][dm-deployment]**


## Recommended Sizing

Workstation/Server Role|OS|CPU|RAM|SSD Disk Size
--- | --- | --- | --- | ---
Client PC|Windows/Linux/Mac|4 Cores i7 Processor or equivalent|16 GB|500 GB
Talend Administration Center|Windows/Linux|4 Cores |8 GB RAM Minimum, 32 GB Recommended for 1000s of Jobs|300GB+ Minimum (for software & logs)
Job Server(s)|Windows/Linux|4 Cores Minimum,8+ Cores Recommended|16 GB RAM Minimum,128 GB Recommended|300+ GB
Centralized Log Server|Windows/Linux|4 Cores Minimum|16 GB RAM|300+ GB
Data Prep & Data Stewardship Server|Windows/Linux|4 Cores Minimum|32 GB RAM|300+ GB
Shared Nexus Server|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|300+ GB
Git Server (Better in Saas Mode)|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|50+ GB
CI Server|Windows/Linux|4 Cores Minimum,8 Cores Recommended|16 GB RAM|300+ GB


<!-- links -->
[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/MkfTXwr0wElt98slxn9TSg/content "Talend Data Management Platform functional architecture Picture"
{:.img-fluid}
[dm-dev]: ./dm-physical-reference-architecture-dev
[dm-test]: ./dm-physical-reference-architecture-test
[dm-prod]: ./dm-physical-reference-architecture-prod
[dm-deployment]: ./dm-depoyment-strategy
