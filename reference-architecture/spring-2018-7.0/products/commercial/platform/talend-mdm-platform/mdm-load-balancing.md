---
title: "HTTP Load Balancer"
creationDate: "02/27/2018"
modifieDdate: "02/28/2018"
product: "dataintegration"
version: "7.0"
reviewer: ""
lastReviewedDdate: "02/27/2018"
latest.revision: 1
author: "Lokesh"
---

## HTTP Load Balancer

- The MDM server distribution does not provide any HTTP load balancer. The load balancer must be installed separately.

- MDM server is compatible with any HTTP load balancer (Hardware or Software) as long as it provides session affinity (i.e. the capability to redirect all the requests concerning a session to the same node)

- All BPM requests directed to a single node
