# Databasify Labs

**Open-source alternative to DigitalOcean Managed Databases, Amazon RDS and Aiven.**

Databasify turns a few Linux servers you own into highly available PostgreSQL, MySQL, MariaDB, MongoDB, Valkey and Redis clusters, with one web UI to run them: the managed database experience, self-hosted, without the per-node markup.

## What you get

- **Start small, scale to a cluster:** a single primary, then standbys with automatic failover and read-only nodes whenever you need them
- **Six engines:** PostgreSQL 17 and 18, MySQL 8.4 and 9.7, MariaDB 11.4 and 11.8, MongoDB 7.0, 8.0 and 9.0, Valkey 8 and 9, Redis 8
- **Safe by default:** TLS everywhere (a CA file is optional), private networking, firewalls and hostnames on your own domain
- **Day-two operations:** backups with point-in-time recovery to any S3-compatible bucket, connection pools, users, metrics, live activity logs and email alerts
- **Easy moves:** migrate from an existing database while it keeps serving traffic, then cut over
- **Hands-off updates:** new engine releases installed in a weekly maintenance window
- **Any server:** bring your own over SSH, or create them on DigitalOcean, Hetzner, Vultr or Linode
- **Any distribution:** Ubuntu 24.04 and 26.04, Debian 12 and 13, Rocky Linux 9 and AlmaLinux 9, SELinux enforcing included

## Projects

| Project | What it is |
|---|---|
| [databasify](https://github.com/databasifylabs/databasify) | The control plane: a Laravel and React app that sets up and runs your clusters over SSH |
| [engines](https://github.com/databasifylabs/engines) | `ghcr.io/databasifylabs/databasify-<engine>`: the official database images, extended with HA and backup tools and a small Go supervisor |

## Get started

On a Linux server with at least 1 GB of memory:

```bash
curl -fsSL https://raw.githubusercontent.com/databasifylabs/databasify/0.x/scripts/install.sh | sudo bash
```

---

If Databasify saves you time, give it a ⭐. It helps others find it.
