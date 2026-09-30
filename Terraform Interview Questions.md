# Terraform Interview Questions

## Core concepts

- Providers
- Resources
- Data sources
- Variables
- Locals
- Outputs
- Modules
- State
- Remote backends
- State locking
- Workspaces
- Import
- Drift
- Plan/apply lifecycle

## Production practices

- Store state remotely with appropriate access control.
- Protect production state from accidental deletion.
- Review plans before production changes.
- Use modules for repeated infrastructure patterns.
- Separate environments without creating uncontrolled configuration duplication.
- Never commit credentials or sensitive state files.

## Scenario questions

1. Terraform detects unexpected drift. What do you check?
2. Two engineers run apply simultaneously. How do you prevent conflicts?
3. An apply fails halfway through. What is your next step?
4. A resource exists manually but not in Terraform. How do you bring it under management?
5. A module change affects 20 services. How do you roll it out safely?
6. How would you implement policy checks before apply?
7. How would you detect infrastructure changes made outside Terraform?
