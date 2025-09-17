# Uptime Kuma Docker Deployment

A complete Docker Compose setup for deploying Uptime Kuma with MySQL database and Caddy reverse proxy with automatic HTTPS.

## 📋 Overview

This deployment includes:

- **Uptime Kuma**: Self-hosted monitoring tool
- **MySQL 9.0**: Database backend for Uptime Kuma
- **Caddy**: Reverse proxy with automatic HTTPS certificates

## 🔧 Prerequisites

- Docker and Docker Compose installed
- Domain name pointing to your server (for HTTPS)
- Ports 80 and 443 available on your server

## 🚀 Quick Start

1. **Clone this repository**

    ```bash
    git clone https://github.com/shaban00/uptimekuma-docker.git
    cd uptimekuma-docker
    ```

2. **Create environment file**

    ```bash
    cp .env.example .env
    ```

3. **Configure environment variables. Edit .env file with your values:**

    ```bash
    nano .env
    ```

4. **Configure Caddy reverse proxy. Edit Caddyfile with your domain:**

    ```bash
    nano Caddyfile
    ```

    Change localhost to your domain. Eg: example.com

5. **Deploy the stack**

    ```bash
    docker compose up -d
    ```
