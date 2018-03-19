### QA, UAT & Production Environment:

#### Simple:
![[2]][2]

*Download a [Visio file][vd-DI-6.4-prod-Simple] that contains this architecture diagram.*

#### Advanced:
![[3]][3]

*Download a [Visio file][vd-DI-6.4-prod-Advanced] that contains this architecture diagram.*

#### Environment Highlights
- Servers shown per role per environment
- We will replicate the servers on the right for each environment
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.
- No GIT is shown here because it is not required in TEST,Pre-Prod and Production Environments
- Data Preparation and Data Stewardship are only going to be installed if customer wants them on-premise.

<!-- links -->
[2]: ./../../../resources/images/di-architecture/DI-Architecture-6.4-Prod-Simple.png "DI Architecture 6.4 - Simple Prod"
[vd-DI-6.4-prod-Simple]: ./../../../resources/templates/visio/di-architecture/DI-Architecture-6.4-Prod-Simple.vsd
[3]: ./../../../resources/images/di-architecture/DI-Architecture-6.4-Prod-Advanced.png "DI Architecture 6.4 - Advanced Prod"
[vd-DI-6.4-prod-Advanced]: ./../../../resources/templates/visio/di-architecture/DI-Architecture-6.4-Prod-Advanced.vsd
