# FIAP - https://www.fiap.com.br/

## Solution Sprint - Fase 04


### Dockerfile

```
podman build . -t <user>//node-web-app

podman run -dt -p 8080:8080/tcp --name my-running-app localhost/<user>/node-web-app
```
