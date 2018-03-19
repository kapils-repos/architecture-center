## Big Data – Physical Reference Architecture for Development

#### Simple Development:
![[0]][0]

*Download a [Visio file][BD-Architecture-6.4-dev-simple] that contains this architecture diagram.*

#### Advanced Development:
![[1]][1]

*Download a [Visio file][BD-Architecture-6.4-advanced] that contains this architecture diagram.*

### Environment Highlights:

- Same as Data Management Platform Reference Architecture
- Servers shown per role
- Network connections and ports not shown here to keep the diagram simple enough to follow
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.
- JobServer deployed on Edge Nodes for Big Data Yarn Client processing.
- JobServers are installed seperate from TAC Servers in Advanced Configuration.

<!-- links -->
[0]: ./../../../resources/images/big-data/BD-Architecture-6.4-dev-simple.png "Big Data Architecture 6.4 for Development - Simple"
[BD-Architecture-6.4-dev-simple]: ./../../../resources/templates/visio/big-data-architecture/BD-Architecture-6.4-dev-simple.vsd
[1]: ./../../../resources/images/big-data/BD-Architecture-6.4-advanced.png "Big Data Architecture 6.4 for Development - Advanced"
[BD-Architecture-6.4-advanced]: ./../../../resources/templates/visio/big-data-architecture/BD-Architecture-6.4-advanced.vsd
