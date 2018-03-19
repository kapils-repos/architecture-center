
### Typical Physical Architecture:

#### DI - Simple Development Architecture:
![[0]][0]

*Download a [Visio file][vd-DI-6.4-dev-Simple] that contains this architecture diagram.*

#### DI - Advanced Development Architecture:
![[1]][1]

*Download a [Visio file][vd-DI-6.4-dev-Advanced] that contains this architecture diagram.*

#### Environment Highlights:
- Servers show per role
- Network connections and ports not shown here to keep the diagram simple enough to follow
- Optional components are shown as yellow dashed boxes
- One Nexus is shared across all environments.  This is the starting point.  The customer needs to justify why they need more than 1 Nexus across the whole deployment.
- GIT is only needed in the development environment and not accessed from other environments.

<!-- links -->
[0]: ./../../../resources/images/di-architecture/di-architecture6.4-simple.png "DI Architecture 6.4 - Simple Dev"
[vd-DI-6.4-dev-Simple]: ./../../../resources/templates/visio/di-architecture/di-architecture6.4-simple.vsd
[1]: ./../../../resources/images/di-architecture/DI-Architecture-6.4-Advanced.png "DI Architecture 6.4 - Advanced Dev"
[vd-DI-6.4-dev-Advanced]: ./../../../resources/templates/visio/di-architecture/DI-Architecture-6.4-Advanced.vsd
