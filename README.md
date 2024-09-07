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
