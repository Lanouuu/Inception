# Inception

**42 School Project**

## Overview

Inception is a system administration project focused on containerization, infrastructure deployment and service configuration using Docker.

The objective is to build a small web infrastructure composed of multiple isolated containers, orchestrated through Docker Compose, while ensuring service communication, data persistence and security.

## Architecture

The infrastructure consists of three main services:

| Service | Role |
|---|---|
| **NGINX** | Web server and HTTPS reverse proxy |
| **WordPress** | Content management system |
| **MariaDB** | Relational database |

Each service runs in its own dedicated container and communicates through a Docker network.

## Technologies

- **Linux / Debian:** System administration and environment configuration.
- **Docker:** Containerization and service isolation.
- **Docker Compose:** Multi-container orchestration.
- **NGINX:** Web server and reverse proxy.
- **WordPress:** Web application deployment.
- **MariaDB:** Database management.
- **TLS / SSL:** HTTPS encryption.
- **Bash:** Automation and configuration scripts.

## Implementation

### 1. Containerization

- Creation and configuration of custom Docker images.
- Service isolation and container lifecycle management.
- Docker Compose orchestration.
- Configuration of inter-container networking.

### 2. Infrastructure Deployment

- Deployment of NGINX, WordPress and MariaDB.
- Configuration of PHP-FPM and database connectivity.
- HTTPS configuration with TLS certificates.
- Reverse proxy configuration.

### 3. Persistence and Security

- Configuration of Docker volumes for persistent data.
- Database and WordPress data management.
- Environment variables and credentials management.
- Network isolation and secure service communication.

## Useful Commands

```bash
# Build and start the infrastructure
docker compose up -d --build

# List running containers
docker compose ps

# Display container logs
docker compose logs -f

# Access a container
docker exec -it <container_name> sh

# Stop the infrastructure
docker compose down

# Stop and remove containers and volumes
docker compose down -v
```

## Skills Acquired

- Linux system administration.
- Docker image creation and management.
- Multi-container orchestration.
- Web server and database configuration.
- Network isolation and service communication.
- HTTPS and TLS configuration.
- Persistent storage management.
- Infrastructure security and troubleshooting.

---

**School:** 42  
**Project:** Inception  
**Status:** Completed
