# n8n + Postgres (Docker)
Requirements:

Docker & Docker Compose

Setup:
1) Copy env file
cp .env.template .env

2) (Optional) Enable init script
chmod +x init-data.sh

3) Start services
docker compose up -d

4) Open n8n
http://localhost:5678

Notes:

1- Data persists in volumes: db_storage, n8n_storage

2- Default timezone: Asia/Riyadh

3- If you don’t use init-data.sh, remove its volume line from postgres.volumes

4- To change the port, edit the ports mapping (e.g. 8080:5678)
