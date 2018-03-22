Wordpress stack with docker with SSL using letsencrypt service with automatic certificate renewal.

# Containers used
* [nginx-proxy](https://github.com/jwilder/nginx-proxy) as frontend proxy
* [docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) used to generate and update SSL certificates and config files for nginx-proxy
* [wordpress:latest](https://hub.docker.com/_/wordpress/) 
* [mysql:5.7](https://hub.docker.com/_/mysql/)

Rename example.env to .env and fill in the variables

