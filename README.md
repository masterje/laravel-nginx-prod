Docker image from Chatgpt for a laravel project prod setup .  This uses Laravel 12 with Mysql.  

Browser
   ↓
Nginx (port 8080)
   ↓
PHP-FPM (port 9000 internally)
   ↓
MySQL


your-project/
│
├── docker-compose.yml
├── nginx/
│   └── default.conf
├── php/
│   └── Dockerfile
└── www/

docker compose up -d --build

In the php container:
docker exec -it laravel_php bash
composer create-project laravel/laravel .



