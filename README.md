# 🐳 Laravel + Docker Stack

[![Docker](https://img.shields.io/badge/Docker-20.10%2B-blue?logo=docker)](https://www.docker.com/)
[![Laravel](https://img.shields.io/badge/Laravel-10%2B-red?logo=laravel)](https://laravel.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-17-blue?logo=postgresql)](https://www.postgresql.org/)

Entorno Docker completo para desarrollo Laravel con Traefik, PostgreSQL, PgAdmin y Portainer.

## 🚀 Instalación rápida

```bash
# Clonar repositorio
git clone https://github.com/VicInfante/login-system.git
cd login-system

# Instalar dependencias (host)
cp .env.example .env
composer install
npm install
composer require laravel/sail --dev

# Iniciar contenedores
docker-compose up -d

# Ejecutar migraciones
docker-compose exec laravel.test php artisan migrate
