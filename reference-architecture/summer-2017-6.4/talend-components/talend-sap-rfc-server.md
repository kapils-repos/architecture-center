---
title: "Talend SAP RFC Server"
creationDate: "02/27/2018"
modifiedDate: "02/28/2018"
product: "dataintegration"
version: "6.4.1"
reviewer: ""
lastReviewedDate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

# Talend SAP RFC Server

![RFC][RFCImage]

Talend SAP RFC Server is a standalone server that acts as a gateway between Talend Studio and an SAP server. It receives IDoc documents from the SAP server and makes them available for processing in Talend Jobs.

- It utilises a JMS queue to collect IDoc documents.
- Talend Data Mapper can be used to parse the IDoc’s.

### Browsing IDoc Types

<img src="./../resources/images/components/sap-rfc.png" alt="SAPRFC" width="100%" height="100%">

### Simple Job Flow

<img src="./../resources/images/components/sap-job.png" alt="SapJob" width="100%" height="100%">

To see how to configure SAP to operate with the Talend SAP RFC Server please click <a href="https://help.talend.com/reader/l4K8UxOw8Sq2gL_98eV_AQ/XTBZ10mfThW6CMwFrWvLdg" target="_blank">Talend Help documentation</a>  

<!-- links -->
[RFCImage]: https://help.talend.com/api/fluidtopicsclient/resources/9g5xugYWkj6RbKCiRpbI6Q/content "RFC Server Architecture"
{:.img-fluid}
