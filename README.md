!(https://github.com/Axe-s/yamdb_final/actions/workflows/yamdb_workflow.yml/badge.svg)

# API для проекта api_yamdb
Проект призван собирать отзывы и оценки на различные произведения
***

### Шаблон .env файла:
* DB_ENGINE=django.db.backends.postgresql
* DB_NAME=postgres
* POSTGRES_USER=<пользователь>
* POSTGRES_PASSWORD=<пароль>
* DB_HOST=db 
* DB_PORT=5432 
***
### Как запустить проект:
Из папки infra запускаем команду:
```
docker-compose up
```

Делаем миграции, создаем суперпользователя и собираем статику:
```
docker-compose exec web python manage.py migrate
docker-compose exec web python manage.py createsuperuser
docker-compose exec web python manage.py collectstatic
```
***

### Документация по работе с проектом находится по адресу:
```
http://localhost/redoc/
```
***
### Авторы проекта:

* Цыганов Даниил
* Сенькин Иван
* Николаев Антон

