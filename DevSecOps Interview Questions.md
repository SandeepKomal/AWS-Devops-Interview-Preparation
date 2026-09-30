# DevSecOps Interview Questions

## Security pipeline

```text
Source
  ↓
Secret Scan
  ↓
SAST
  ↓
Dependency / SCA
  ↓
Build
  ↓
Container Scan
  ↓
SBOM / Provenance
  ↓
IaC Scan
  ↓
Deploy
  ↓
DAST / Runtime Validation
```

## Know the difference

- **SAST:** analyzes source/code without running the application.
- **SCA:** identifies vulnerable or risky third-party dependencies.
- **DAST:** tests a running application.
- **Secret scanning:** detects credentials/tokens in source and artifacts.
- **IaC scanning:** checks infrastructure definitions for insecure configurations.
- **Container scanning:** checks image packages and configuration for vulnerabilities.

## Kubernetes security

Prepare:

- RBAC
- least-privilege ServiceAccounts
- NetworkPolicies
- Pod Security Standards
- secrets management
- admission policies
- image provenance/signing
- namespace isolation

## Scenario

A critical vulnerability is discovered after an image has reached production.

Explain how you identify affected deployments, assess exposure, rebuild/replace the image, verify the fix, rotate credentials if necessary and prevent recurrence through pipeline and runtime controls.
