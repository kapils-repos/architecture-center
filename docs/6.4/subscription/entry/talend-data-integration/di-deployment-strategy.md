
### Environments Deployment Strategy

#### Simple:
![[4]][4]

*Download a [Visio file][vd-DI-6.4-prod-Simple] that contains this architecture diagram.*

#### Advanced:
![[5]][5]

*Download a [Visio file][vd-DI-6.4-prod-Advanced] that contains this architecture diagram.*

#### Highlights:
- The GIT in the SDLC server is only accessible from the Development Environment.  Other environments cannot access GIT.
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.
- Continous Integration can be setup if going with Advanced setup

<!-- links -->
[4]: ./../../../resources/images/di-architecture/deployment-di-simple.png "DI Deployment 6.4 - Simple"
[vd-DI-6.4-prod-Simple]: ./../../../resources/templates/visio/di-architecture/deployment-di-simple.vsdx
[5]: ./../../../resources/images/di-architecture/deployment-di-advanced.png "DI Deployment 6.4 - Advanced"
[vd-DI-6.4-prod-Advanced]: ./../../../resources/templates/visio/di-architecture/deployment-di-advanced.vsdx
