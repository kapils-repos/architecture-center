---
title: "Talend Activity Monitoring Console (AMC)"
creationDate: "02/27/2018"
modifiedDate: "02/28/2018"
product: "dataintegration"
version: "6.5"
reviewer: ""
lastReviewedDate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## Talend Activity Monitoring Console (AMC)

![Talend Activity Monitoring Console][AMC]

Talend Activity Monitoring Console is an add-on tool integrated in the studio and in Talend Administration Center for monitoring Talend Jobs and projects.It helps Talend product administrators or users to achieve enhanced resource management and improved process performances through a convenient graphical interface and a supervising tool. It provides detailed monitoring capabilities that can be used to consolidate the collected activity monitoring information, understand the underlying component and Job interaction, prevent faults that could be unexpectedly generated and support system management decisions.

In general the functionalities are :
- Batch process monitoring
- Log information about each execution of a DI job
- Jobs can automatically write information to the AMC DB or File
- TAC and Studio can access information within the AMC DB or File through the Activity Monitoring Console GUI

### Technical Details:
- Three database tables or files:
	**Stats**
	**Logs**
	**Flow Meter**
- Schema of each table can be extended to add more columns for extra info
- Common Databases Supported
- Volume of data stored in these 3 tables are directly related to number of tasks and frequency of executions
- Developer must design Jobs to manage the size and performance of these tables or files

To read and understand the functionalities of AMC in detail please read <a href="https://help.talend.com/reader/9XL7dCVn5F8r97d6FjjmhQ/MDauhq9nl1m0FXZX~aHp9Q" target="_blank">Talend Help documentation</a>


<!-- links -->
[AMC]: https://help.talend.com/api/fluidtopicsclient/resources/slgCAC2hH9AGN8ZMrbZAQA/content "Talend Activity Monitoring Console"
{:.img-fluid}
