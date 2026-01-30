# Orvex Cloud (Orvex, LLC)

Welcome to the **Orvex Cloud** GitHub organisation — maintained by **Orvex, LLC**.

Orvex Cloud is a lightweight PaaS for everyday developers and small teams who want **predictable pricing**, **always-on services**, and managed primitives (deployments, PostgreSQL, cronjobs, and serverless functions) without hyperscale complexity.

> An org by **doranteseduardo**: https://github.com/doranteseduardo

## What you’ll find here

This organisation hosts the code and tooling behind Orvex Cloud, including (depending on what’s public at any given time):

- Platform components and services
- SDKs / client libraries
- Examples and templates
- Documentation and guides

## What Orvex Cloud provides

- **Projects (Deployments)** — always-on services for APIs, web apps, and workers  
- **Databases (PostgreSQL)** — managed Postgres with automated daily backups and retention  
- **Cronjobs (Scheduled Tasks)** — scheduled execution with retries and timeouts  
- **Serverless (Functions)** — fast endpoints for webhooks, lightweight APIs, and short tasks  

## Principles

- **Always-on by default** — no sleeping on inactivity.
- **Simple monthly tiers** — predictable costs.
- **Resource limits per service** — CPU/RAM limits are enforced per workload.
- **Stability first** — we manage capacity to keep performance consistent.

## Access model

Orvex Cloud is **capacity-managed**. Accounts and upgrades are approved to prevent over-subscription and maintain reliability.

If you’d like access, apply via the Orvex Cloud website and include a short description of what you’re building.

## Infrastructure (high level)

We run on dedicated bare metal with NVMe storage and enforce per-service resource limits. Deployment storage is **persistent**. PostgreSQL includes **automated daily backups** with plan-based retention.

## Support

If you have a question or you’ve found an issue, please open an issue in the relevant repository (when enabled), or use the support/contact channel listed on the website.

## Security

Found a security vulnerability? Please **don’t** open a public issue.  
Report it privately with details and reproduction steps, and we’ll respond as quickly as possible.

## License

Unless stated otherwise in a repository, each project should include a `LICENSE` file describing its terms.
