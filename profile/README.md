# Orvex Cloud

> Maintained by **Orvex, LLC** · by [@doranteseduardo](https://github.com/doranteseduardo)

Orvex Cloud is a Docker-based PaaS built for developers and small teams who want **predictable pricing**, **always-on workloads**, and a full suite of managed primitives — without hyperscale complexity or surprise bills.

Deploy from GitHub or a ZIP upload, get an automatic `*.orvex.cloud` subdomain, and manage everything through the dashboard or a REST API.

---

## What Orvex Cloud provides

### Services
Always-on Docker container deployments from any GitHub repo or ZIP archive. Automatic subdomain routing, real-time build logs, env vars (AES-encrypted), custom domains, and GitHub webhook auto-deploy. Includes:

- **Web services** — HTTP containers with Traefik routing and SSL
- **Static sites** — served via a shared Nginx gateway
- **Background workers** — no port exposure, no routing; pure compute

### Databases
Fully managed containers with automated daily backups and plan-based retention:

| Engine | Backup method |
|--------|--------------|
| PostgreSQL | `pg_dump` + PostgREST sidecar (`rest-*.orvex.cloud/rest/v1`) |
| MySQL | `mysqldump` |
| MongoDB | `mongodump` |
| Redis | Passive RDB snapshot |

Every PostgreSQL database gets a **PostgREST sidecar** automatically — JWT-authenticated REST API out of the box.

### Functions
Always-warm serverless using a shared pool model — no cold starts. Four runtimes available:

- **Bun** (TypeScript/JavaScript)
- **Deno** (TypeScript/JavaScript)
- **Python 3.11**
- **Go**

Handlers follow the Web Fetch API: `Request → Response`.

### Cronjobs
Scheduled tasks with full execution history, manual triggers, and enable/disable toggles. Cron expressions, configurable timeouts, and per-tier rate limits.

### Object Storage
Per-bucket MinIO instances, S3-compatible API, Traefik SSL endpoints, and access key management through the dashboard or API.

### More primitives

- **Persistent Volumes** — named Docker volumes shared across services within an org
- **Env Groups** — org-scoped shared environment variable sets, attached to one or many services; merged at build time
- **Service Dependencies** — declare startup ordering with cycle detection and automatic topological sort
- **App Templates** — 10 one-click stacks: Next.js, Express+Postgres, Django, Rails, FastAPI, Go API, WordPress, Ghost, Redis Worker, Meilisearch
- **Branch Previews** — automatic preview environments per branch push
- **Inter-service DNS** — project-scoped service discovery

---

## Pricing

| Tier | Monthly | Services | Databases | Functions | Cronjobs | Storage Buckets |
|------|---------|----------|-----------|-----------|----------|-----------------|
| **Free** | $0 | 1 × 0.25 CPU / 512 MB | 1 × 500 MB | 3 × 1K calls/day | 3 × 100/day | 2 × 5 GB |
| **Starter** | $29 | 5 × 0.5 CPU / 1 GB | 3 × 2 GB | 10 × 10K calls/day | 10 × 500/day | 5 × 25 GB |
| **Pro** | $99 | 20 × 1 CPU / 2 GB | 10 × 10 GB | 50 × 100K calls/day | 50 × 2K/day | 15 × 100 GB |
| **Scale** | $299 | 50 × 2 CPU / 4 GB | 20 × 30 GB | 100 × 500K calls/day | 100 × unlimited | 30 × 500 GB |

**Add-ons:** Service Pack +5 ($8/mo) · DB Pack +3 ($12/mo) · Function Pack +20 ($5/mo) · Storage Pack +25 GB/bucket ($4/mo)

Billing is org-level — one Stripe subscription, all resources inherit the org's tier.

---

## Principles

- **Always-on by default** — no sleeping on inactivity.
- **Simple monthly tiers** — no per-request metering surprises.
- **Enforced resource limits** — CPU and RAM caps are applied per workload.
- **Stability first** — capacity-managed to keep performance consistent across tenants.

---

## Access

Orvex Cloud is **capacity-managed**. Accounts are approved to prevent over-subscription. If you'd like access, apply via the Orvex Cloud website and include a short description of what you're building.

---

## What's in this organisation

Depending on what's public at any given time:

- Platform source (API, dashboard, infrastructure config)
- SDKs and client libraries
- Example apps and one-click templates
- Documentation and setup guides

---

## Support

Open an issue in the relevant repository (when enabled), or use the support channel listed on the Orvex Cloud website.

## Security

Found a vulnerability? **Please don't open a public issue.**  
Report it privately with details and reproduction steps — we'll respond as quickly as possible.

## License

Each repository includes a `LICENSE` file describing its terms.
