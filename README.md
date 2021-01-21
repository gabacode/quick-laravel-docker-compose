# Docker-compose container for quick deployment

# Includes:
PHP7.4<br>
Nginx<br>
phpMyAdmin<br>

# QuickStart
## INSTALL LARAVEL
```
composer create-project laravel/laravel .
```

## Change .env file with:
```
DB_CONNECTION=mysql<br>
DB_HOST=mysql<br>
DB_PORT=3306<br>
DB_DATABASE=homestead<br>
DB_USERNAME=homestead<br>
DB_PASSWORD=secret<br>
```
In order to use php artisan, call the full path from inside the container<br>
Example:<br>
```
docker-compose exec php php /var/www/html/artisan config:cache
```
