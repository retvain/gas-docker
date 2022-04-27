## Docker for gas-api project

## to run:
### clone to parent directory gas-api
`cd gas-docker`

`docker-compose up -d`

`docker-compose exec php-fpm bash`

`cd gas-api-operator-arm`
`composer install`
`php artisan migrate:refresh --seed --force`

`cd ../gas-api-operator-arm`
`composer install`
`php artisan migrate:refresh --seed --force`

`ln -s /var/www/gas-api-operator-arm/vendor/voskhod /var/www/gas-api-organizator-arm/vendor`
