---
title: "Talend Master Data Management Platform (MDM)"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---
# Talend Master Data Management Platform (MDM)

## Introduction
Talend MDM is a model-driven, non intrusive solution easily adaptable to specific business needs and quick to implement. It has been specifically developed to address the challenges of creating and managing master data for all types of organizations where data is hosted under various formats in various systems and can be extremely volatile.

**Talend Master Data Management** (MDM) groups all the company's master data of the company in a central hub. This standardized repository provides, via the use of Data Models, the prerequisites against which data and updates are validated.

Talend MDM ensures the right people have the right tools to centrally model and manipulate master data. Its master data governance features are available through two different user interfaces: one is an administration tool called Talend Studio and the other is a web-based interface called Talend MDM Web User Interface.

The chart below illustrates the main building blocks (Talend Studio, Web browser ,MDM server & MDM database) of Talend MDM.

![[MDM-Picture]][MDM-Picture]

Below page describes in detail the architecture that make up the Talend MDM Platform and its Logical Architecture, Physical Architecture & Sizing guidelines.

# Architecture

## Talend Master Data Management Embedded Architecture
![0][0]

### Key Features
- Data model creation
- Security / Audit
- Event management
- Data quality
- Data stewardship
- Survivorship
- Multi-domain
- BPM and workflow
- Batch and real-time integration
- MDM REST API


## Logical Reference Architecture

Talend MDM architecture can be broken down into functional blocks that enable interaction between users and the MDM Hub and their corresponding IT needs. For more details on the individual components of Logical Architecture please refer <a href="https://help.talend.com/reader/nuYRviXq8Y02nVMd3jI~UA/H3CnbCOoJWdRL3MZG_a13Q" target="_blank">Talend Help documentation</a>.

The following chart illustrates the main architectural functional blocks.

![alt text][logical-architecture-picture]


## Physical Reference Architecture

### Key Components
- **[MDM Server][mdm-server]**
- **[MDM Physical Storage][mdm-physical-storage]**
- **[MDM Server Architecture][mdm-server-architecture]**
- **[MDM Server Clustering][mdm-server-clustering]**
- **[MDM Load Balancing][mdm-load-balancing]**
- **[MDM Real Time][mdm-real-time]**

### Environments

- **[Development Environment][mdm-dev]**

- **[Testing Environment][mdm-test]**

- **[Pre-Prod & Production Environment][mdm-prod]**

- **[MDM – High Availability and Real-Time][mdm-ha]**


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
Database Cluster|Depends on database technology, existing volume and rate of growth of Master Data. Always planned for 3 – 5 years of data growth.

<!-- links -->
[logical-architecture-picture]: https://help.talend.com/api/fluidtopicsclient/resources/Z97AnDV9Euhy1nEC0BG28A/content "Talend MDM functional architecture picture"
{:.img-fluid}
[MDM-Picture]: https://help.talend.com/api/fluidtopicsclient/resources/yOmWawmJThZgatqPm768IQ/content "Talend Enterprise MDM Picture"
{:.img-fluid}
[0]: ./../../../../resources/images/mdm/MDM-Embedded-Arch.png "Talend Master Data Management Embedded Architecture"

[mdm-server]: ./mdm-server
[mdm-physical-storage]: ./mdm-physical-storage
[mdm-server-architecture]: ./mdm-server-architecture
[mdm-server-clustering]: ./mdm-server-clustering
[mdm-load-balancing]: ./mdm-load-balancing
[mdm-real-time]: ./mdm-real-time

[mdm-dev]: ./mdm-physical-reference-architecture-dev
[mdm-test]: ./mdm-physical-reference-architecture-test
[mdm-prod]: ./mdm-physical-reference-architecture-prod
[mdm-ha]: ./mdm-physical-reference-architecture-ha
