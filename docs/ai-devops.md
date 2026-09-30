# AI / Agentic DevOps Interview Guide

AI-related DevOps questions should be answered as infrastructure and security problems, not only as model questions.

## Topics

- Model serving and inference latency
- GPU scheduling basics
- Token/request cost
- Caching and batching
- RAG deployment considerations
- Agent identity
- Tool permissions
- Auditability
- Data boundaries
- Human approval for high-impact actions
- Rate limits and blast-radius controls

## Scenario

An AI agent is allowed to restart Kubernetes workloads.

Discuss:

1. Identity and authentication.
2. Exact RBAC permissions.
3. Namespace/resource scope.
4. Allowed tools and arguments.
5. Approval requirements for production.
6. Audit logging.
7. Rate limiting.
8. Rollback and emergency disablement.

The key interview skill is showing how automation can be powerful without becoming unrestricted production access.
