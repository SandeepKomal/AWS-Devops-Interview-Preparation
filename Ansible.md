# Ansible Interview Questions

## What is Ansible?
Ansible is an agentless automation tool for configuration management, application deployment and operational automation. Linux hosts commonly use SSH and Windows hosts can use WinRM.

## Idempotency
An idempotent task produces the desired state without making unnecessary changes when it is run repeatedly.

## Inventory vs dynamic inventory
Static inventory lists hosts explicitly. Dynamic inventory discovers hosts from a source such as AWS.

## Playbook vs role
A playbook orchestrates automation. A role packages reusable tasks, handlers, templates, variables and defaults.

## Common modules
package, service, copy, template, file, user, command and shell. Prefer purpose-built modules over shell/command when possible.

## Secrets
Ansible Vault encrypts sensitive values/files. For production, compare it with external secret managers such as AWS Secrets Manager or HashiCorp Vault.

## Interview scenarios
1. How do you make a playbook safe to run repeatedly?
2. How do you manage secrets without committing them?
3. How would you target EC2 instances by tags?
4. How would you roll out a change gradually?
5. Why might a task work manually but fail in Ansible?
6. How would you design Ansible for hundreds of hosts?

## Production scenario
A configuration change breaks 5% of production servers. Explain how you stop the rollout, identify affected hosts, restore the previous state and prevent recurrence.
