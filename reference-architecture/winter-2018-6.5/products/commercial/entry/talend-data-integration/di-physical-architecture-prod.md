---
title: "QA, UAT & Production Environment"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.5"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## QA, UAT & Production Environment

### Simple
<img src="./../../../../resources/images/di-architecture/data-integration-physical-architecture-test-prod-simple-6.5.svg" alt="DI Architecture 6.5 - Simple Prod" width="100%" height="100%">

*Download a [Visio file][vd-DI-6.5-prod-Simple] that contains this architecture diagram.*

### Advanced
<img src="./../../../../resources/images/di-architecture/data-integration-physical-architecture-test-prod-advanced-6.5.svg" alt="DI Architecture 6.5 - Advanced Prod" width="100%" height="100%">

*Download a [Visio file][vd-DI-6.5-prod-Advanced] that contains this architecture diagram.*

### Environment Highlights
- Servers shown per role per environment
- We will replicate the servers on the right for each environment
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.
- No GIT is shown here because it is not required in TEST,Pre-Prod and Production Environments
- Data Preparation and Data Stewardship are only going to be installed if customer wants them on-premise.

<!-- links -->
[vd-DI-6.5-prod-Simple]: ./../../../../resources/visio/di-architecture/data-integration-physical-architecture-6.5.vsdx
[vd-DI-6.5-prod-Advanced]: ./../../../../resources/visio/di-architecture/data-integration-physical-architecture-6.5.vsdx
