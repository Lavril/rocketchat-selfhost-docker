# 🚀 Self-Hosted Rocket.Chat Deployment Guide

This repository provides a step-by-step guide to deploying **[Rocket.Chat](https://www.rocket.chat)** by Docker on your own infrastructure.  
Ideal for teams or organizations looking to keep full control over their communication platform.

### ⚠️ Important Notice

> **Air-gapped servers (offline environments) are only supported with a paid Rocket.Chat plan.**  
> The **Starter** plan **does not work** in such setups. See [this forum](https://forums.rocket.chat/t/starter-plan-on-air-gapped-workspace/22384/8) for details.

---

## 📌 Features

- ✅ Self-hosted deployment (with Docker)
- ✅ Secure (HTTPS via Let's Encrypt)
- ✅ MongoDB integration
- ✅ Reverse proxy setup
- ✅ Systemd service configuration
- ✅ Optional LDAP / SSO integration

---

## 🧰 Prerequisites

- A Linux server (tested on Ubuntu 22.04)
- Root or sudo access
- Domain name (e.g. `chat.example.com`)
- [Optional] Docker & Docker Compose installed

---

## 🚀 Installation

> There are two options: **Docker-based** or **Manual installation**.

### Option 1: Docker (recommended)

```bash
git clone https://github.com/your-username/rocketchat-selfhost-guide.git
cd rocketchat-selfhost-guide/docker
cp .env.example .env
docker-compose up -d
