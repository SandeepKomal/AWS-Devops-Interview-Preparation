# AWS Interview Questions

## Networking
**VPC:** A logically isolated AWS network where you define IP ranges, subnets, routing and network connectivity.

**Public vs private subnet:** A public subnet has a route to an Internet Gateway. A private subnet does not have a direct route to an Internet Gateway. Private workloads can use controlled egress such as NAT Gateway or service-specific VPC endpoints.

**Route table:** Determines where network traffic is sent.

**Security Group vs NACL:** Security Groups are stateful and attached to ENIs/resources. Network ACLs are stateless rules applied at the subnet boundary.

**Internet Gateway vs NAT Gateway:** An Internet Gateway provides VPC connectivity to/from the internet for appropriately routed resources. NAT Gateway allows private resources to initiate outbound internet connections without accepting unsolicited inbound connections.

## Compute and scaling
- EC2: virtual compute
- AMI: template used to launch EC2 instances
- Launch Template: reusable EC2 launch configuration
- Auto Scaling Group: maintains desired capacity and replaces unhealthy instances
- EBS: block storage for EC2

## Load balancing
**ALB:** Layer 7 HTTP/HTTPS routing, host/path rules and application-aware features.

**NLB:** Layer 4 TCP/UDP/TLS load balancing for high-performance network traffic.

**Target group:** Logical set of targets receiving load-balancer traffic.

## S3
S3 is object storage. Know versioning, lifecycle policies, storage classes, encryption, Block Public Access, bucket policies, Object Ownership, replication and VPC endpoints.

## IAM
Prefer short-lived credentials and IAM roles over long-lived access keys. Apply least privilege and understand trust policies versus permission policies.

## RDS
Know Multi-AZ for availability/failover, read replicas for read scaling, automated backups, parameter groups, security groups and encryption.

## Scenario questions
1. Private EC2 cannot reach S3 — what do you check?
2. ALB returns 502 — how do you isolate the failure?
3. An ASG keeps replacing instances — what evidence do you collect?
4. AWS costs increased suddenly — how do you investigate?
5. A developer requests AdministratorAccess — how do you design the required permissions?
6. An application needs multi-AZ resilience — what components must be redundant?
7. How would you design DR across AWS regions?

## Interview rule
For senior questions, explain **architecture → security → reliability → cost → operational trade-offs**, not just the service definition.
