---
title: "Environments Deployment Strategy"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Environments Deployment Strategy

### Simple

<img src="./../../../../resources/images/di-architecture/data-integration-deployment-architecture-simple-7.0.svg" alt="DI Deployment 7.0 - Simple" width="100%" height="100%">

*Download a [Visio file][vd-DI-7.0-prod-Simple] that contains this architecture diagram.*

### Advanced

<img src="./../../../../resources/images/di-architecture/data-integration-deployment-architecture-advanced-7.0.svg" alt="DI Deployment 7.0 - Advanced" width="100%" height="100%">

*Download a [Visio file][vd-DI-7.0-prod-Advanced] that contains this architecture diagram.*

### Highlights
- The GIT in the SDLC server is only accessible from the Development Environment.  Other environments cannot access GIT.
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.
- Continous Integration can be setup if going with Advanced setup

<!-- links -->
[vd-DI-7.0-prod-Simple]: ./../../../../resources/visio/di-architecture/data-integration-deployment-architecture-7.0.vsdx
[vd-DI-7.0-prod-Advanced]: ./../../../../resources/visio/di-architecture/data-integration-deployment-architecture-7.0.vsdx
