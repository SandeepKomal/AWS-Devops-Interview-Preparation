# Git & GitHub Interview Questions

## Core

- clone, fetch, pull and push
- branch and merge
- rebase
- cherry-pick
- revert vs reset
- tags
- protected branches
- pull requests
- CODEOWNERS
- GitHub Actions
- environments and approvals

## DevOps scenarios

1. A bad commit reached main. How do you safely revert it?
2. Two branches have conflicting changes. How do you resolve them?
3. A secret was committed. What is the response?
4. How do you protect the production branch?
5. How do you implement CI checks before merge?
6. How do you promote the same immutable artifact through environments?
7. GitHub Actions needs AWS access. How would you avoid long-lived AWS access keys?

## Senior topic

Explain why the source commit, build artifact/image digest and deployed version should be traceable as one chain:

```text
Commit SHA → Build → Artifact/Image Digest → Deployment → Runtime
```
