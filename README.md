
docker run -d -p 3000:8080 --add-host=host.docker.internal:host-gateway -v open-webui:/app/backend/data --env-file openwebui.env --name open-webui ghcr.io/open-webui/open-webui:main
docker run --rm -it -p 4566:4566 -p 4510-4559:4510-4559 localstack/localstack
docker run -d --name redis-stack -p 6379:6379 -p 8001:8001 redis/redis-stack:latest

WIP
- logout
- oidc redirection on kat 

