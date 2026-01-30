# Orvex Cloud (Orvex, LLC)

Orvex Cloud is a lightweight PaaS built for everyday developers and small teams who want predictable pricing, always-on services, and managed building blocks (deployments, PostgreSQL, cronjobs, and serverless functions) without hyperscale complexity.

We operate as **Orvex, LLC**.

## What we build

Orvex Cloud provides a small set of primitives you can combine to run real projects:

- **Projects (Deployments)** — always-on services for APIs, web apps, and workers
- **Databases (PostgreSQL)** — managed Postgres with automated daily backups and retention
- **Cronjobs (Scheduled Tasks)** — scheduled execution with retries and timeouts
- **Serverless (Functions)** — fast endpoints for webhooks, lightweight APIs, and short tasks

## Design principles

- **Always-on by default**: no sleeping on inactivity.
- **Predictable pricing**: simple monthly tiers.
- **Resource limits per service**: CPU/RAM are assigned and enforced per workload.
- **Capacity-first operations**: we prioritise stability and consistent performance over raw scale.

## Access model

Orvex Cloud is **capacity-managed**. Accounts and upgrades are approved to prevent over-subscription and keep the platform reliable for everyone.

If you’d like access, apply via the website and include a short description of what you’re building.

## Infrastructure

We run on dedicated bare metal with NVMe storage and enforce per-service resource limits (CPU/RAM). Storage for deployments is **persistent**. PostgreSQL includes **automated daily backups** with plan-based retention.

## Repositories in this organisation

You’ll find:

- core platform services (control plane / data plane)
- SDKs and client libraries
- examples and templates
- docs and guides

## Getting started

- Visit the product website to view pricing and apply for access.
- Once approved, you’ll be able to create Projects, Databases, Cronjobs, and Functions from the dashboard/API (depending on what’s enabled for your account).

## Support

For support and account questions, open an issue in the appropriate repository (or use the contact method listed on the website, if provided).

## Security

If you believe you’ve found a security issue, please **do not** open a public issue.
Instead, contact us privately with details and a reproduction path. We will respond as quickly as possible.

## License

Unless stated otherwise in a given repository, projects under this organisation will include a LICENSE file defining usage terms.
