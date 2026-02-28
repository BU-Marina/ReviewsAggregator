# Проект ReviewsAggregator

[![CI](https://github.com/BU-Marina/ReviewsAggregator/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/BU-Marina/ReviewsAggregator/actions/workflows/ci.yml)

Собираются пользовательские отзывы на произведения по категориям (книги, фильмы и музыка).

## Шаблон наполнения env-файла

    DB_ENGINE=<engine>
    DB_NAME=<name>
    POSTGRES_USER=<username>
    POSTGRES_PASSWORD=<password>
    DB_HOST=<host>
    DB_PORT=<port>

    DEBUG=<debug>
    SECRET_KEY=''

## Запуск приложения в контейнерах

Выполнить из директории с файлом docker-compose_local.yaml

```
docker-compose -f docker-compose_local.yml up -d --build
```

Остановить и удалить контейнеры и volumes:

```
docker-compose -f docker-compose_local.yml down -v
```
