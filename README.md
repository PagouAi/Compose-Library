# 🐳 Docker Compose Library

A curated collection of ready-to-use Docker Compose files for common development
and infrastructure tools. Spin up services in seconds with minimal
configuration.

### ⚠️ Reminder

> These Docker Compose files are intended **only for local development and
> testing**.\
> They are **not** production-ready and should **not be used in production
> environments**.\
> Using them in production is **at your own risk and responsibility**.

## 🚀 What’s Inside

This repository includes Docker Compose setups for:

| Stack                  | Services                                          | Use Case                                     |
| ---------------------- | ------------------------------------------------- | -------------------------------------------- |
| `mysql-admin`          | MySQL + phpMyAdmin                                | MySQL database with web admin interface      |
| `postgres-admin`       | PostgreSQL + pgAdmin                              | PostgreSQL database with web admin interface |
| `postgres-redis`       | PostgreSQL + Redis                                | Database with caching layer                  |
| `kafka-postgres-redis` | Kafka + Zookeeper + PostgreSQL + Redis + Kafka UI | Event streaming with database and cache      |
| `observability-stack`  | PostgreSQL + Redis + NATS + Prometheus + Grafana  | Full monitoring and observability setup      |

> Each service is in its own folder with isolated `docker-compose.yml` files for
> modular use.

## 🧑‍💻 Getting Started

### Prerequisites

Windows/Linux:

- [Docker](https://www.docker.com/products/docker-desktop)

MacOs:

- [Orbstack](https://orbstack.dev/)

### Usage

```bash
cd kafka-postgres-redis
docker compose up -d
```

To stop the service:

```bash
docker compose down
```

## 🛠 Customization

Each Compose file is intended to be a starting point. You can:

- Update environment variables (e.g., passwords, ports)
- Mount custom volumes for data persistence
- Link multiple services via Docker networks

## 🤝 Contributing

Contributions are welcome! Feel free to submit:

- New Compose setups
- Improvements to existing configurations
- Documentation updates

### Contribution Guide

1. Fork this repository
2. Add your service under a new folder
3. Create a PR with a short description and usage notes

## ❤️ Credits

Maintained by Pagou.ai. Inspired by the awesome Docker community.
