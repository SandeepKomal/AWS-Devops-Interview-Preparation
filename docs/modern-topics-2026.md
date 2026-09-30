# Modern AWS DevOps Interview Topics — 2026

## GitOps

Know the difference between push-based CD and pull-based GitOps. Prepare source of truth, reconciliation, drift, secrets, rollback and multi-cluster promotion.

Typical question:

> Why would an organization use Argo CD or Flux instead of having Jenkins run kubectl directly?

## Platform Engineering

Know Internal Developer Platforms, golden paths, Backstage, self-service environments, platform APIs and developer-experience metrics.

Current platform-engineering research highlights developer productivity, agentic AI capabilities and cost governance as major priorities. 

## AI and agentic infrastructure

Prepare model-serving basics, inference latency, GPU scheduling concepts, RAG deployment concerns, agent permissions, tool/API access, cost governance and auditability.

MCP and agent tooling also introduce questions around least privilege, exposed tool surfaces and centralized authorization.

## FinOps

Be ready to discuss rightsizing, autoscaling, Spot vs On-Demand, Savings Plans, storage lifecycle policies, NAT Gateway cost, VPC endpoints, tagging and workload unit economics.

AWS's current CloudOps service scope includes Cost Explorer, Cost and Usage Reports and Savings Plans alongside EC2, ECR, ECS, EKS, Lambda and Bedrock.

## Observability and SRE

Move beyond naming CloudWatch or Datadog. Explain metrics, logs, traces, events, SLIs, SLOs, error budgets and alerting based on user impact.

```text
Metrics → Logs → Traces → Events
              ↓
            SLOs
              ↓
        Error budgets
              ↓
        Alerting policy
```

## Security and software supply chain

Prepare least-privilege IAM, workload identity, secrets management, SBOMs, SAST/SCA/DAST, container scanning, admission policy and artifact signing.

## EKS depth

Go beyond Pods and Deployments: networking/CNI, IP exhaustion, workload identity, ingress/load balancing, HPA/VPA, PDBs, topology spread, autoscaling and node lifecycle.

## AWS architecture trade-offs

Prepare ECS vs EKS, NAT Gateway vs VPC endpoints, Terraform vs native AWS IaC, managed vs self-managed databases and security/reliability trade-offs.

## Focus order

Build depth around AWS + Kubernetes + Terraform + CI/CD + Security + Observability + Reliability + Cost. Then layer GitOps, platform engineering and AI infrastructure on top.
