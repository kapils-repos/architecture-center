---
title: "Big Data – Physical Reference Architecture for Development"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Big Data – Physical Reference Architecture for Development

### Simple Development
<img src="./../../../../resources/images/big-data/big-data-physical-architecture-dev-simple-7.0.svg" alt="Big Data Architecture 7.0 for Development - Simple" width="100%" height="100%">

*Download a [Visio file][BD-Architecture-7.0-dev-simple] that contains this architecture diagram.*

### Advanced Development
<img src="./../../../../resources/images/big-data/big-data-physical-architecture-dev-advanced-7.0.svg" alt="Big Data Architecture 7.0 for Development - Advanced" width="100%" height="100%">

*Download a [Visio file][BD-Architecture-7.0-advanced] that contains this architecture diagram.*

### Environment Highlights

- Same as Data Management Platform Reference Architecture
- Servers shown per role
- Network connections and ports not shown here to keep the diagram simple enough to follow
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.
- JobServer deployed on Edge Nodes for Big Data Yarn Client processing.
- JobServers are installed seperate from TAC Servers in Advanced Configuration. 

<!-- links -->
[BD-Architecture-7.0-dev-simple]: ./../../../../resources/visio/big-data-architecture/big-data-physical-architecture-7.0.vsdx
[BD-Architecture-7.0-advanced]: ./../../../../resources/visio/big-data-architecture/big-data-physical-architecture-7.0.vsdx
