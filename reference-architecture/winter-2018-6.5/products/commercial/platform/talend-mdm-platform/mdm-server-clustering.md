---
title: "MDM Server Clustering, Cache and Indexing"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "6.5"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## MDM Server Clustering, Cache and Indexing

### Clustering
Balance load on several MDM server instances and provide High Availability – Bonita is not HA

![0][0]


### Cache
- Hibernate 2nd level cache (EhCache)
- Cache replication using JMS messages

### Indexing
Hibernate search index (Lucene) replication

![1][1]



<!-- links -->
[0]: ./../../../../resources/images/mdm/mdm-server-clustering.png "Clustering"
[1]: ./../../../../resources/images/mdm/mdm-server-clustering-lucene.png "indexing"
