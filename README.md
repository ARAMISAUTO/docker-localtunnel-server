# localtunnel-server-nginx

Docker Compose setup for running a Localtunnel server behind a SSL Nginx reverse proxy.

## Usage

```
git clone https://github.com/ARAMISAUTO/localtunnel-server-nginx.git
cd localtunnel-server-nginx
docker-compose up
```

SSL certificate (`server.crt`) and key (`server.key`) must reside in project's `ssl` subdirectory.
