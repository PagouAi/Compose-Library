# 🐳 Docker Compose Library

A curated collection of ready-to-use Docker Compose files for common development
and infrastructure tools. Spin up services in seconds with minimal
configuration.

## 🚀 What’s Inside

This repository includes Docker Compose setups for:

- 📦 **Databases**
  - PostgreSQL
  - MySQL
  - Redis

- 🔧 **Dev Tools**
  - pgAdmin
  - phpMyAdmin

- 📊 **Monitoring & Logging**
  - Prometheus + Grafana

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
cd postgresql-redis
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

Maintained by [YourName or Organization]. Inspired by the awesome Docker
community.
