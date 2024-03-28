# Steps to run this example

1. Clone this repo
```bash
https://github.com/budhasanjeev/react-docker-example.git
```

2. Go inside the directory
```bash
cd laravel-docker-example
```

3. Build the image
```bash
docker-compose build
```

4. Run the container
```bash
docker-compose up -d
```

5. To composer install
```bash
docker-compose exec laravel-app bash
```

```bash
composer install
```

6. Run artisan migration
```bash
docker-compose exec laravel-app bash
```

```bash
php artisan migrate
```

