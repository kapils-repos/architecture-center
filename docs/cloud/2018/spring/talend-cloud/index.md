---
title: "Talend Integration Cloud"
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

The Talend Integration Cloud service application enables data and file transfer, data integration, and access to shared data sources for web users. Talend Studio is plugged into this web application for developers to publish data integration Jobs to the web application, make them available to web users, and run them in the Cloud. Once a connection is established, any update in your scenario from Talend Studio can be pushed to the Cloud right away.

# Architecture

The Logical Architecture give us a high level view of various components that make up the platform and Physical Architecuture provides guidelines for various deployment environments.

## Talend Platform

## Logical Reference Architecture

![alt text][Logical Architecture]

For more details on the individual components of Logical Architecture please refer [Talend Help documentation][logical-architecture-details]. 

## Physical Reference Architecture

### Guiding Principles (Same as for Data Integration):
- We will have 3 environments as per our best practices
- SDLC is achived via code promotion pipelines

### Environments:

- **[Development Environment][tc-dev]**

- **[Pre-Prod & Production Environment][tc-prod]**


## Recommnded Sizing

Workstation/Server Role|OS|CPU|RAM|SSD Disk Size
--- | --- | --- | --- | ---
Client PC|Windows/Linux/Mac|4 Cores i7 Processor or equivalent|16 GB|500 GB
Remote Engine(s)|Windows/Linux|4 Cores Minimum,8+ Cores Recommended|16 GB RAM Minimum,128 GB Recommended|300+ GB
Shared Nexus Server|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|300+ GB
Git Server (Better in Saas Mode)|Windows/Linux|4 Cores Minimum|8 GB RAM Minimum|50+ GB

Note: 
- You need 1 Cloud or 1 Remote Engine at a minimum per environment
For Big Data:
- Remote Engines must be installed on Edge Nodes
- Remote Engines must be running on Linux OS
- Remote Engines Cluster
- Configured in Cloud dashboard
- Remote Engines are optional
- Additional Sizing info on Cloud and Remote Engines, refer to Talend Integration Cloud Sizing Cloud Engine <2017 version>

<!-- links -->

[logical-architecture-details]: https://help.talend.com/reader/xMKe8U4ggRRAlmi97fpXxg/AUsVGExbYMAX_kDGRskD6w "TIC architecture"

[Logical Architecture]: https://help.talend.com/api/fluidtopicsclient/resources/aZcggahzbsJ7hCacqBNnog/content "Talend Integration Cloud"

[tc-dev]: ./tc-physical-reference-architecture-dev.md
[tc-prod]: ./tc-physical-reference-architecture-prod.md 
