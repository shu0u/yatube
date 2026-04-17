# API для Yatube

## Описание

Проект API для Yatube.

С помощью API можно:
- работать с публикациями;
- оставлять комментарии;
- подписываться на авторов;
- получать данные с JWT-аутентификацией.

## Как запустить проект

Клонировать репозиторий и перейти в него в командной строке:

    git clone https://github.com/shu0u/api-final-yatube.git
    cd api-final-yatube

Cоздать и активировать виртуальное окружение:

    python -m venv venv
    source venv/Scripts/activate

Установить зависимости из файла requirements.txt:

    pip install -r requirements.txt

Перейти в папку с проектом:

    cd yatube_api

Выполнить миграции:

    python manage.py migrate

Запустить проект:

    python manage.py runserver

## Примеры запросов

Получить список публикаций:

    GET /api/v1/posts/

Создать публикацию:

    POST /api/v1/posts/

Получить JWT-токен:

    POST /api/v1/jwt/create/
