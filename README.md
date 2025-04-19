
# Exploration project on [Open WebUI](https://openwebui.com/)

## Stateless with s3 / pgvector / redis
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --env-file openwebui.env --name open-webui ghcr.io/open-webui/open-webui:main
docker run --rm -it -p 4566:4566 -p 4510-4559:4510-4559 localstack/localstack
docker run -d --name redis-stack -p 6379:6379 -p 8001:8001 redis/redis-stack:latest

## OpenIdConnect
With Microsoft EntraId

## Use authenticated api from another application
Web site (on same host with nginx reverse-proxy)

##### WIP
- logout failed
- oidc redirection on kat 

