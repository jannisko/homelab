


```bash
set -a
source secrets.env
source .env

envsubst < services/media-server/transmission.env.template > services/media-server/transmission.env
envsubst < services/git-server/drone.env.template > services/git-server/drone.env

docker-compose -f services/media-server/docker-compose.yml up -d
docker-compose -f services/git-server/docker-compose.yml up -d
```