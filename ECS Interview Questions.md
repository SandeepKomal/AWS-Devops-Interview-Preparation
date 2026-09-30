# Amazon ECS Interview Questions

## What is ECS?
Amazon Elastic Container Service is a managed AWS container orchestration service. Tasks can run on EC2 capacity or AWS Fargate.

## Core components
Cluster: logical ECS grouping.
Task definition: versioned configuration describing containers, images, CPU/memory, networking, logging and IAM roles.
Task: running instance of a task definition.
Service: maintains desired task count and supports deployment and load-balancer integration.

## Networking
Know awsvpc networking, ENIs, subnets, security groups, service discovery and load-balancer integration.

## Task roles
A task role grants the application permissions to call AWS APIs. An execution role is used by ECS/Fargate infrastructure for operations such as pulling images and sending logs. Do not confuse the two.

## EC2 vs Fargate
EC2 capacity gives more control over underlying instances. Fargate removes host management. Choose based on operational ownership, workload characteristics, cost, capacity control and integrations.

## Deployments
Prepare rolling deployments, blue/green deployments, health checks, deployment circuit breakers and rollback.

## Observability
Know CloudWatch Logs, metrics, container health checks, load-balancer target health and application telemetry.

## Security
Prepare task IAM roles, security groups, private subnets, ECR access, secrets injection and least privilege.

## Scenarios
1. ECS tasks continuously stop. What do you inspect?
2. Tasks cannot pull an ECR image. What permissions and network checks do you perform?
3. ALB returns 503 while tasks show Running. What is your investigation path?
4. Fargate cost is increasing. What sizing data do you inspect?
5. A task needs S3 access. How do you grant it without static credentials?
6. A deployment is unhealthy. How do you stop or roll it back safely?
7. When would ECS be an operational fit compared with Kubernetes?
