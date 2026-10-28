# Databasify Labs

**Open-source, self-hosted database clusters on your own servers.**

Databasify turns a few Linux servers into highly available PostgreSQL, MySQL, MariaDB, Valkey and Redis clusters, with one web UI to run them. Your servers, your data, no per-database fees.

## What you get

- **Clusters, not single instances:** a primary with standbys, automatic failover and read-only nodes
- **Five engines:** PostgreSQL 17 and 18, MySQL 8.4, MariaDB 11.4 and 11.8, Valkey 8 and 9, Redis 8
- **Safe by default:** TLS everywhere, private networking, firewalls and hostnames on your own domain
- **Day-two operations:** backups with point-in-time recovery to any S3-compatible bucket, connection pools, users, metrics, logs and alerts
- **Easy moves:** migrate from an existing database while it keeps serving traffic
- **Any server:** bring your own over SSH, or create them on DigitalOcean, Hetzner, Vultr or Linode
- **Any distribution:** Ubuntu 24.04 and 26.04, Debian 12 and 13, Rocky Linux 9 and AlmaLinux 9

## Projects

| Project | What it is |
|---|---|
| [databasify](https://github.com/databasifylabs/databasify) | The control plane: a Laravel and React app that sets up and runs your clusters over SSH |
| [Engine images](https://github.com/orgs/databasifylabs/packages) | `ghcr.io/databasifylabs/databasify-<engine>`: the official database images, extended with HA and backup tools and a small Go supervisor |

## Get started

```bash
curl -fsSL https://raw.githubusercontent.com/databasifylabs/databasify/main/scripts/install.sh | sudo bash
```

## License

Databasify is open source under the [AGPL-3.0](https://github.com/databasifylabs/databasify/blob/main/LICENSE). Use it, change it and self-host it freely.

---

If Databasify saves you time, give it a ⭐. It helps others find it.
