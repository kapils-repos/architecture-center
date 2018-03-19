## Data Management – Deployment Strategy

#### Simple:
![[0]][0]

*Download a [Visio file][deployment-dm-simple] that contains this architecture diagram.*

### Environment Highlights:

- The GIT in the SDLC server is only accessible from the Development Environment.  Other environments cannot access GIT.
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.

#### Advanced:
![[1]][1]

*Download a [Visio file][deployment-dm-advanced] that contains this architecture diagram.*

### Environment Highlights:

- The GIT in the SDLC server is only accessible from the Development Environment.  Other environments cannot access GIT.
- Only Nexus Releases and Snapshots repositories are accessible to TEST and PRE-PROD environments.
- Only Releases repository is accessible from PROD environment.
- Nexus access can be controlled by user privileges and firewall/proxy.
- Jenkins, Commandline, CI Builder and Nexus part of same server.


<!-- links -->
[0]: ./../../../resources/images/data-management/deployment-dm-simple.png "Simple Deployment Strategy"
[deployment-dm-simple]: ./../../../resources/templates/visio/dm-architecture/deployment-dm-simple.vsd
[1]: ./../../../resources/images/data-management/deployment-dm-advanced.png "Advanced Deployment Strategy"
[deployment-dm-advanced]: ./../../../resources/templates/visio/dm-architecture/deployment-dm-advanced.vsd
