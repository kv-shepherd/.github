# KubeVirt Shepherd

**KubeVirt Shepherd** (also known as **kv-shepherd**) is an open-source application for teams managing KubeVirt virtual machines. It brings VM requests, approval policies, scoped access and audit records together across Kubernetes/KubeVirt clusters.

[KubeVirt Shepherd official website](https://kv-shepherd.io/) · [KubeVirt Shepherd 中文官网](https://kv-shepherd.io/zh/) · [Documentation](https://github.com/kv-shepherd/shepherd/blob/main/docs/README.md)

## Explore or install

The [browser demo](https://demo.kv-shepherd.io/) uses simulated data and operations. No account is needed: switch roles, explore requests and approvals, and reset the demo. It does not provision real VMs or connect to live consoles.

For real VM operations, run a self-hosted installation connected to your Kubernetes/KubeVirt environment. The [deployment guide](https://github.com/kv-shepherd/shepherd/blob/main/docs/DEPLOYMENT.md) covers Helm on Kubernetes and Docker Compose on a host, including configuration requirements.

## Project status

Shepherd is currently **Alpha**. Review the [release notes](https://github.com/kv-shepherd/shepherd/releases) and evaluate compatibility, permissions, storage, networking and authentication in your environment before connecting shared workloads. Approval requirements depend on the operation and environment policy; actions that do not require approval still need the appropriate permissions.

## Repositories

| Repository | Responsibility |
| --- | --- |
| [shepherd](https://github.com/kv-shepherd/shepherd) | The main application: Go API and workers, web UI, API contracts and project documentation. |
| [helm-charts](https://github.com/kv-shepherd/helm-charts) | Official Helm chart and configuration guidance for installing Shepherd on Kubernetes. |
| [kv-shepherd.io](https://github.com/kv-shepherd/kv-shepherd.io) | Go vanity import metadata for the `kv-shepherd.io/shepherd` module path. |
| [.github](https://github.com/kv-shepherd/.github) | This public organization profile and community information. |

## Get involved

- [Read the documentation](https://github.com/kv-shepherd/shepherd/blob/main/docs/README.md) for architecture and usage guidance.
- [Report an issue](https://github.com/kv-shepherd/shepherd/issues) with the workflow, environment and steps needed to reproduce it.
- [Read the contribution guide](https://github.com/kv-shepherd/shepherd/blob/main/CONTRIBUTING.md) before proposing changes.
- [Read the security policy](https://github.com/kv-shepherd/shepherd/blob/main/SECURITY.md) for vulnerability reporting.

KubeVirt Shepherd is released under the [Apache License 2.0](https://github.com/kv-shepherd/shepherd/blob/main/LICENSE).
