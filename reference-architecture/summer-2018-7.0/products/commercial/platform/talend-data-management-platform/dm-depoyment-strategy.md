---
title: "Data Management – Deployment Strategy"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Data Management – Deployment Strategy

### Simple:
<img src="./../../../../resources/images/data-management/data-management-deployment-architecture-simple-7.0.svg" alt="Simple Deployment Strategy" width="100%" height="100%">

*Download a [Visio file][deployment-dm-simple] that contains this architecture diagram.*

### Environment Highlights

- The GIT in the SDLC server is only accessible from the Development Environment.  Other environments cannot access GIT.
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.

### Advanced
<img src="./../../../../resources/images/data-management/data-management-deployment-architecture-advanced-7.0.svg" alt="Advanced Deployment Strategy" width="100%" height="100%">

*Download a [Visio file][deployment-dm-advanced] that contains this architecture diagram.*

### Environment Highlights

- The GIT in the SDLC server is only accessible from the Development Environment.  Other environments cannot access GIT.
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.
- Jenkins, Commandline, CI Builder and Nexus part of same server. 


<!-- links -->
[deployment-dm-simple]: ./../../../../resources/visio/dm-architecture/data-management-deployment-architecture-7.0.vsdx
[deployment-dm-advanced]: ./../../../../resources/visio/dm-architecture/data-management-deployment-architecture-7.0.vsdx
