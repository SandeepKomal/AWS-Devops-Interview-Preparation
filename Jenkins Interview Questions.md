# Jenkins Interview Questions

## Core
- Controller vs agent
- Declarative vs Scripted Pipeline
- Multibranch Pipeline
- Credentials management
- Shared Libraries
- Webhooks
- Artifacts
- Parallel stages
- Pipeline approvals
- Ephemeral agents

## Production design

A secure pipeline should generally look like:

```text
Commit
  ↓
Checkout
  ↓
Tests
  ↓
SAST / SCA / Secret Scan
  ↓
Build
  ↓
Container Scan
  ↓
Artifact Registry
  ↓
Deploy
  ↓
Health / Smoke Tests
  ↓
Promote or Roll Back
```

## Scenario questions

1. Jenkins build succeeds but deployment fails. What do you inspect?
2. Jenkins agents are exhausted. How do you scale execution?
3. A credential appears in logs. What do you do immediately?
4. How do you prevent deploying an unscanned image?
5. How do you implement approval only for production?
6. How do you make pipelines reusable across 50 services?
7. How would you migrate a Jenkins deployment to GitOps?
