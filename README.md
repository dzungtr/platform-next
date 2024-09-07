# platform-next
Template for building next organization technology stack following platform engineering practice

Platform engineering is a modern practice, mutual from DevOps culture. However, for an organization to implement Platform engineering practice in culture. It usually is expensive and take a lot of time. This project aims to create a boilerplate to bootstrap infrastructure. It helps Technology holder to create a platform for developers to do their job, deploy their features to production and do not worry about infrastructure specific specs. Embracing automating, consistency and security.

The stucture of the projects will look like:
- Components: networks, observability, VPC, instances, … (k8s & cloud)
- Cloud providers: Implementation manifest specific by cloud provider
- Secrets vault
- Policy: reconciliation policy, network policy, security policy, ...
- Templates
- Sources: application deployment manifest
- Scripts/cli: action command
- Agents: Crossplane, ArgoCD, ...


## Getting started

### Prerequisite
These software need to be installed and well setup in local machine
- [Nix shell](https://nixos.org/download/#download-nix)
- [Direnv](https://direnv.net/)
- Container run time. eg: Docker desktop ^4.30.0

### 1. Install software

Navigate to the repo folder, all software will be automatically installed by direnv and nix setup

```
~/p/dzungtr> cd platform-next/
direnv: loading ~/project/dzungtr/platform-next/.envrc
direnv: using nix
direnv: export <SOME env var>
```

List of softwares installed can be tracked in `default.nix` file. The lab uses `kind` as k8s cluster distribution to set up local easily. More information, you can reference here https://kind.sigs.k8s.io/