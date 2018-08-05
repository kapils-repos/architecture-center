---
title: "Talend MDM Physical Storage"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Talend MDM Physical Storage

### Purpose
- Master Data
- Staging Data
- MDM Journal
- MDM System data
- Cross-referencing (unused but still required)
- Bonita journal / history (optional)

### Technical Details
- Server component
- Number of relational databases supported
- One set of Databases / Schemas required per MDM server – may be multiple Master / Staging areas*
- Database can be very large, depending on the volume of Master Data records4
- Should be clustered for HA
