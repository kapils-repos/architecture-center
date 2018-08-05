---
title: "Data Management – Physical Reference Architecture for Development"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.5"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Data Management – Physical Reference Architecture for Development

### Development
<img src="./../../../../resources/images/data-management/data-management-physical-architecture-dev-advanced-6.5.svg" alt="DM Architecture 6.5 for Development" width="100%" height="100%">

*Download a [Visio file][DM-Architecture-6.5-Dev] that contains this architecture diagram.*

### Environment Highlights

- Servers shown per role
- Network connections and ports not shown here to keep the diagram simple enough to follow
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.

<!-- links -->
[DM-Architecture-6.5-Dev]: ./../../../../resources/visio/dm-architecture/data-management-physical-architecture-6.5.vsdx