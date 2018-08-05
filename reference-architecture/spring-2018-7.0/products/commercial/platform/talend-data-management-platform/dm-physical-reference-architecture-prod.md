---
title: "Data Management – Physical Reference Architecture for Pre-Prod and Production Data Management Platform"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Data Management – Physical Reference Architecture for Pre-Prod and Production

### Pre-Prod & Prod Environment
<img src="./../../../../resources/images/data-management/data-management-physical-architecture-preprod-prod-7.0.svg" alt="DM Architecture 7.0 for Pre-Pro & Prod" width="100%" height="100%">

*Download a [Visio file][DM-Architecture-7.0-Prod] that contains this architecture diagram.*

### Data Preparation and Stewardship Expanded View

<img src="./../../../../resources/images/data-management/data-management-physical-architecture-dp-ds-expanded-7.0.svg" alt="Data Preparation and Stewardship Expanded View" width="100%" height="100%">

### Environment Highlights

- Servers shown per role per environment
- We will replicate the servers on the right for each environment
- No Nexus shown here because it is on our SDLC Server.
- Central Log Server is not shown here.
- Data Prep and Data Stewardship are not shown here.
- Failover device is generally Apache Httpd, VIP, or a Load Balancer.  However, not all Load Balancer are tested by Talend.  Hence, limitations will exist.

### Advanced Configurations
- **[Setting up High Availability][ha]**

- **[Using Virtual Job Servers][vjs]**

<!-- links -->
[DM-Architecture-7.0-Prod]: ./../../../../resources/visio/dm-architecture/data-management-physical-architecture-7.0.vsdx
[ha]: ./tac-ha-availability
[vjs]: ./virtual-job-servers
