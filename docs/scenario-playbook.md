# Production Scenario Playbook

## AWS

### 1. Application is slow after a deployment
Walk through recent changes, ALB metrics, target health, application logs, CPU/memory, database latency, downstream dependencies and rollback.

### 2. Private EC2 cannot reach S3
Check route tables, NAT/VPC endpoint design, security controls and DNS. Explain when an S3 endpoint can avoid NAT dependency.

### 3. AWS bill suddenly increases
Find the service/resource driving the change, compare usage over time, inspect recent deployments and apply a preventive control.

## Kubernetes

### 4. Pod is Pending
Check events, resource requests, taints, affinity, topology constraints and node availability.

### 5. Pod is CrashLoopBackOff
Inspect current and previous logs, pod events, probes, configuration, secrets, dependencies and recent changes.

### 6. Pods cannot obtain IP addresses
Investigate CNI/IP capacity, subnet free addresses, ENI limits and node placement.

### 7. Deployment causes errors
Stop promotion, inspect rollout history, isolate the failing version, execute a controlled rollback and add a prevention control.

## CI/CD

### 8. Pipeline succeeds but deployment is broken
Explain why pipeline success is not application health. Add rollout status, readiness checks and post-deploy smoke tests.

### 9. Jenkins agents are exhausted
Inspect queue depth, executors, labels, workload duration and concurrency. Consider ephemeral agents.

### 10. Secret appears in build logs
Treat it as compromised: revoke/rotate, investigate exposure, remove it from source/history when necessary and fix credential handling.

## Terraform

### 11. Terraform plan shows unexpected drift
Determine whether the change was manual, provider-related or state-related. Review code and state before import/revert/update.

### 12. Terraform apply fails halfway through
Inspect the failed resource and state. Do not blindly rerun destructive actions; determine what exists and whether the next plan is safe.

## Observability

### 13. CPU is normal but users see latency
Inspect p95/p99 latency, request rate, saturation, downstream calls, database latency and traces.

### 14. Too many alerts
Group related symptoms, alert on user-impacting SLOs and remove noisy alerts that do not require action.

## Security

### 15. Container image has a critical vulnerability
Determine exploitability and exposure, identify the dependency/layer, patch or rebuild, re-scan and define a future policy.

### 16. Developer asks for cluster-admin
Clarify the operation and grant only the required Kubernetes permissions. Use a dedicated service account/role for recurring automation.

## Platform engineering

### 17. Developers complain Kubernetes is too complex
Propose a golden path with self-service templates, standard security/observability defaults and platform-owned interfaces.

### 18. Platform team wants GitOps
Discuss source of truth, reconciliation, auditability, secrets, rollback and promotion between environments.

## AI infrastructure

### 19. AI service is expensive and slow
Measure latency, request volume, token usage, concurrency and utilization. Consider caching, batching, smaller models and autoscaling.

### 20. Agent needs production tool access
Define tool boundaries, identity, authorization, audit logs, approvals and blast-radius controls before access is enabled.
