## 👋 Welcome to itflow 🚀

IT documentation and ticketing system for MSPs

## 📋 Description

IT documentation and ticketing system for MSPs

## 🚀 Services

- **app**: itfloworg/itflow:latest

### Infrastructure Components

- **db**: Mariadb database


## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/itflow/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/itflow" ~/.local/srv/docker/itflow
cd ~/.local/srv/docker/itflow
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install itflow
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
DB_USER_PASS=changeme_db_password
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:62068

## 📂 Volumes

- `./volumes/data/itflow` - Data storage
- `./volumes/data/db/mariadb/itflow` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
