# Ansible, Terraform and CI/CD Questions

## Terraform

- Why use a remote backend?
- How do you detect and handle drift?
- How do you structure reusable modules?
- How do you protect production state?
- How would you promote infrastructure changes across environments?

## Ansible

- Controller vs managed node?
- Inventory vs dynamic inventory?
- Idempotency?
- Role vs playbook?
- Vault vs external secrets manager?
- How do you make Ansible safe for production?

## Jenkins / GitHub Actions

- Controller vs agent?
- Multibranch Pipeline?
- Shared Library?
- Ephemeral runners?
- Artifact promotion?
- Approval gates?
- Secret handling?
- How do you prevent deployment after a failed security gate?

## Senior scenario

A Terraform change creates infrastructure, Jenkins builds the image, a scanner reports a critical vulnerability and the deployment is already queued. Explain the gates, artifact identity, approval model and rollback path.
