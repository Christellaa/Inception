# Inception
42 School project aimed at building multiple, isolated services using Docker.

The services included are:
- Nginx as the server
- MariaDB as the database
- Wordpress as the website/CMS

## Skills developed
- Containerization with Docker
- Automatic service deployment and initialization with Docker Compose
- Microservices architecture
- Bash scripts
- Docker secrets
- Service interconnection via custom networks
- Persistent storage using Docker volumes
- Generate SSL certificates

## How to run
1. Install Docker
2. Change secrets in `secrets` folder
3. Copy/paste .env.tpl to .env and modify the placeholders, inside `srcs` folder
4. Change the placeholders at line `14` in `srcs/requirements/nginx/Dockerfile` file with your CN and UID
5. Change the placeholder at line `27` in `srcs/requirements/nginx/conf/server.conf` file with your server name
6. `make` in project root folder
