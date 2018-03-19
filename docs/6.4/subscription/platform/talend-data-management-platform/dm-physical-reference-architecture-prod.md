## Data Management – Physical Reference Architecture for Pre-Prod and Production

#### Pre-Prod & Prod Environment:
![[2]][2]

*Download a [Visio file][DM-Architecture-6.4-Prod] that contains this architecture diagram.*

### Environment Highlights:

- Servers shown per role per environment
- We will replicate the servers on the right for each environment
- No Nexus shown here because it is on our SDLC Server.
- Central Log Server is not shown here.
- Data Prep and Data Stewardship are not shown here.
- Failover device is generally Apache Httpd, VIP, or a Load Balancer.  However, not all Load Balancer are tested by Talend.  Hence, limitations will exist.

### Advanced Configurations:
- **[Setting up High Availability][ha]**

- **[Using Virtual Job Servers][vjs]**

<!-- links -->
[2]: ./../../../resources/images/data-management/DM-Architecture-6.4-Prod.png "DM Architecture 6.4 for Pre-Pro & Prod"
[DM-Architecture-6.4-Prod]: ./../../../resources//templates/visio/dm-architecture/DM-Architecture-6.4-Prod.vsd
[ha]: ./tac-ha-availability.md
[vjs]: ./virtual-job-servers.md
