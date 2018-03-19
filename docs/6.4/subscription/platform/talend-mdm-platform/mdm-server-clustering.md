### MDM Server Clustering, Cache and Indexing

#### Clustering:
Balance load on several MDM server instances and provide High Availability – Bonita is not HA

![0][0]


#### Cache:
- Hibernate 2nd level cache (EhCache)
- Cache replication using JMS messages

#### Indexing:
Hibernate search index (Lucene) replication

![1][1]



<!-- links -->
[0]: ./../../../resources/images/mdm/mdm-server-clustering.png "Clustering"
[1]: ./../../../resources/images/mdm/mdm-server-clustering-lucene.png "indexing"
