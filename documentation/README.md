# AWS Resource Inventory

| Resource | Name | Configuration |
|---|---|---|
| VPC A | `ewb-vpc-a` | `10.10.0.0/16` |
| VPC B | `ewb-vpc-b` | `10.20.0.0/16` |
| Public subnet | `ewb-a-public` | `10.10.1.0/24` |
| Private subnet A | `ewb-a-private` | `10.10.2.0/24` |
| Private subnet B | `ewb-b-private` | `10.20.1.0/24` |
| Bastion | `ewb-bastion` | `10.10.1.10` |
| Application A | `ewb-app-a` | `10.10.2.10` |
| Application B | `ewb-app-b` | `10.20.1.10` |
| Peering connection | `ewb-a-b-peer` | VPC A ↔ VPC B |

**Note:** This is the planned resource inventory. Confirm actual resource names and IP addresses in AWS before marking the deployment complete.

