# Docker-compose container for quick deployment

## Includes:
PHP7.4 and MySQL<br>
Nginx<br>
phpMyAdmin<br>

## INSTALL LARAVEL
```
composer create-project laravel/laravel .
```

## Change .env file with:
```
DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=homestead
DB_USERNAME=homestead
DB_PASSWORD=secret
```
In order to use php artisan, call the full path from inside the container<br>
Example:<br>
```
docker-compose exec php php /var/www/html/artisan config:cache
```
