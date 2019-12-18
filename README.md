# moloch-cluster-cfn
Create a load-balanced, auto-scaled Moloch cluster in AWS using CloudFormation
---
This CloudFormation template will deploy an auto-scaled and load-balanced cluster of [Moloch](https://molo.ch) full packet capture instances, enhanced with [Suricata](https://suricata-ids.org/), listening on UDP port 4789 (VXLAN). 
It also creates a [VPC traffic mirroring target](https://docs.aws.amazon.com/vpc/latest/mirroring/traffic-mirroring-target.html) pointing to the load balancer. You can create [filters](https://docs.aws.amazon.com/vpc/latest/mirroring/traffic-mirroring-filter.html) and [mirroring sessions](https://docs.aws.amazon.com/vpc/latest/mirroring/traffic-mirroring-session.html) to monitor traffic from your EC2 instances using a web interface.
