---
title: "Typical Physical Architecture (MDM - DEV Advanced)"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Typical Physical Architecture (MDM - DEV Advanced)

### Development
<img src="./../../../../resources/images/mdm/mdm-physical-architecture-dev-7.0.svg" alt="MDM Architecture 7.0 for Development" width="100%" height="100%">

*Download a [Visio file][MDM-Architecture-7.0-dev] that contains this architecture diagram.*

### Environment Highlights

- Servers shown per role
- Network connections and ports not shown here to keep the diagram simple enough to follow
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.

<!-- links -->
[MDM-Architecture-7.0-dev]: ./../../../../resources/visio/mdm-architecture/mdm-physical-architecture-7.0.vsdx
