# Azure Secure Landing Zone

A production-grade Azure landing zone implementation following Microsoft Cloud Adoption Framework (CAF) principles — built with Zero Trust security, automated governance, and full Terraform IaC.

## What This Demonstrates

- **Management Group hierarchy** — enterprise governance at scale
- **Subscription topology** — platform, identity, connectivity, workload separation
- **Hub-spoke networking** — centralised connectivity with Azure Firewall
- **DNS architecture** — private DNS zones, custom resolvers
- **Identity and access** — Zero Trust RBAC, PIM, managed identities
- **Policy framework** — guardrails enforced before workloads arrive
- **Security baseline** — Defender for Cloud, Sentinel, centralised monitoring
- **IaC automation** — entire environment deployable via single Terraform run

## Architecture Overview
Management Group (Root)
├── Platform
│   ├── Identity Subscription
│   ├── Connectivity Subscription (Hub VNet, Firewall, DNS)
│   └── Management Subscription (Log Analytics, Defender)
└── Workloads
├── Production Subscription
└── Development Subscription
## Documentation

- [Management Group Design](docs/01-management-group-design.md)
- [Subscription Topology](docs/02-subscription-topology.md)
- [Hub-Spoke Networking](docs/03-hub-spoke-networking.md)
- [DNS Architecture](docs/04-dns-architecture.md)
- [Identity and Access](docs/05-identity-access.md)
- [Policy Framework](docs/06-policy-framework.md)
- [Security Baseline](docs/07-security-baseline.md)

## Built With

Terraform | Azure DevOps | GitHub Actions | Azure Policy | Microsoft Sentinel | Defender for Cloud

## Author

Senior Software Engineer — ex-Microsoft ODSP Security team.  
Built HSM-based cryptographic infrastructure at fleet scale.  
Specialising in Cloud Security Architecture for regulated industries.
