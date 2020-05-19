


```bash
set -a
source secrets.env
source .env

docker-compose -f services/media-server/docker-compose.yml up -d
```