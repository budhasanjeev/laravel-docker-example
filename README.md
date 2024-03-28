# Steps to run this example

1. Clone this repo
```bash
https://github.com/budhasanjeev/laravel-docker-example.git
```

2. Navigate inside the project directory
```bash
cd laravel-docker-example
```

3. Build the docker images
```bash
docker-compose build
```

4. Run the container
```bash
docker-compose up -d
```

5. Run composer install
```bash
docker-compose exec laravel-app bash
composer install
```

6. Run artisan migration
```bash
docker-compose exec laravel-app bash
ln -s .env.local .env
php artisan migrate
```

7. Create application key
```bash
docker-compose exec laravel-app bash
php artisan key:generate
```

