# localtunnel-server-nginx

Docker Compose setup for running a Localtunnel server behind a SSL Nginx reverse proxy. It uses the [localtunnel-server](https://github.com/localtunnel/server) and [localtunnel-nginx](https://github.com/localtunnel/nginx) Docker images.

## Usage

```sh
git clone https://github.com/ARAMISAUTO/localtunnel-server-nginx.git
cd localtunnel-server-nginx
docker-compose up
```

SSL certificate (`server.crt`) and key (`server.key`) must reside in project's `ssl` subdirectory.
You can use the following command Iin order to create a self-signed certificate :

```sh
openssl req -x509 -nodes -days 365 -newkey rsa:2048 -keyout ./ssl/server.key -out ./ssl/server.crt
```
