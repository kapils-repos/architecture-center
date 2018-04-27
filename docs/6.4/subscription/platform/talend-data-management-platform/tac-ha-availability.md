## TAC High Availability

![HA](./../../../resources/images/data-management/ha.png)

Talend High Availabulity configuration provides operational continuity of task scheduling. If one TAC is stopped, tasks will continue to be scheduled by another job conductor/scheduler.

### Pre-requisites:
Talend Platform Product (Not available in Talend Data Integration)
All TAC servers and TAC DB servers must be synchronised up to the second. Use NTP and atomic clocks to synchronize time on all servers up to the second.

### Configuration:
- Follow instructions in product [documentation][ha-setup] 
- Both TAC’s connect to same TAC/Quartz database
- Under Job Conductor Parameters in TAC, both TACs use shared drive for:
      Generated jobs folder
      Task logs folder

### Constraints/Limitations:
- Only Job Conductor/Quartz Scheduler is supported as HA (Active – Active) – this is automatically done by Quartz
- TAC GUI and all other functionalities are not supported under HA. Hence, administrators will need to always connect to the same TAC.
- Do NOT configure Active - Active load balancing on TAC – this is not supported.  Only expose one TAC to any sort of client at any given time  
- If High Availability of the TAC web application and / or MetaServlet is required, a network failover device e.g. some load balancers / proxies can be used to achieve and Active – Passive configuration
- Child applications of TAC e.g. Drools Guvnor are also not Highly Available


To read in detail about High Availability please click [link][ha-doc] 

<!-- links -->
[ha-doc]: https://help.talend.com/reader/~KLJE0VIvwYIdHMHvmTVlQ/zK0seROd1hFxvY~F~9EmBw "High Availability Details"
[ha-setup]: https://help.talend.com/reader/~KLJE0VIvwYIdHMHvmTVlQ/MEOdB_xT868zSMBXx34mlA?section=sect-install-setting_up_high_availability "Setting up High Availability"
