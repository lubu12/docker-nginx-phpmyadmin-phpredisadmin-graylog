# phpMyAdmin + phpRedisAdmin + Graylog via Nginx reverse proxy

Run phpMyAdmin, phpRedisAdmin and Graylog using Nginx as reverse proxy via docker-compose

Tested at AWS EC2 and RDS - Amazon Linux 2

## Reference
phpMyAdmin + phpRedisAdmin via Nginx: https://github.com/lubu12/docker-nginx-phpMyAdmin-phpRedisAdmin

Graylog via Nginx: https://github.com/lubu12/docker-graylog

## Sample .env
```
NGINX_VERSION=mainline-alpine
NGINX_PORT=80
DOCKER_NGINX_PORT=8080
PHP_FPM_VERSION=7.3-fpm-alpine
HTML_VOLUME=/var/www/html
PMA_HOSTS=YOUR_DB_HOSTNAME(S)
PMA_ABSOLUTE_URI=http://YOUR_HOSTNAME/phpMyAdmin/
GRAYLOG_URL=http://YOUR_HOSTNAME/graylog/
```

## URL to access phpMyAdmin and phpRedisAdmin
```
http://YOUR_HOSTNAME/phpMyAdmin
http://YOUR_HOSTNAME/phpRedisAdmin
http://YOUR_HOSTNAME/graylog
```
