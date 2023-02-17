# DSO-1466-CI-runners-deployment
A repository for CI runners deployment

## Sumary
We need a way to configure GitHub Actions runners more easily and use an automated task.

## Technical details

- Runners should be installed on a cloud instance/VM.
- GitHub Actions runner can be installed on a per-project or per-organization basis. This Ansible Role should install it either way.
- The runner authentication token should be passed in as a command-line argument:

```
[...] -e RUNNER_AUTHENTICATION_TOKEN=<value>
```

## Expected outcomes

- A repository for CI runners deployment is created.
- New runners can be deployed easily with the new playbook.
