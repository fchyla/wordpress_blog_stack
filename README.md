Wordpress stack with docker-compose with SSL using letsencrypt service with automatic certificate renewal.

![alt-text](https://github.com/fchyla/wordpress_blog_stack/raw/master/wordpress-docker-stack.png "HLD")

# Overview
* [nginx-proxy](https://github.com/jwilder/nginx-proxy) as frontend proxy
* [docker-letsencrypt-nginx-proxy-companion](https://github.com/JrCs/docker-letsencrypt-nginx-proxy-companion) used to generate and update SSL certificates and config files for nginx-proxy
* [wordpress:latest](https://hub.docker.com/_/wordpress/) 
* [mysql:5.7](https://hub.docker.com/_/mysql/)

Includes import of SQL db via the WP_IMPORT_SQL_IMPORT_FILE variable and WP_CONTENT_VOLUME to mount "wp-content" directory on persistent storage

> wp-content contains all user-supplied content, all that you upload to the blog is stored there
> post content is stored in the wordpress database

# HOWTO

Rename example.env to .env, make sure it is in the same place as the compose file, and fill in the variables

WP_IMPORT_SQL_IMPORT_FILE and WP_CONTENT_VOLUME should be absolute or relative to the docker-compose file

Run _docker-compose config_ to preview the config
