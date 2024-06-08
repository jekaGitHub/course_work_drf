# course_work_drf

Бэкенд-часть SPA веб-приложения "Трекер полезных привычек".

Технологии:

- python 3.11
- postgresql
- Redis
- os
- dotenv
- API

Используемые библиотеки:

- Django
- djangorestframework
- djangorestframework-simplejwt
- celery
- django-celery-beat
- pillow
- psycopg2-binary
- python-dotenv
- redis
- django-cors-headers
- drf-yasg

Инструкция для развертывания проекта:

1. Клонировать проект:
  https://github.com/jekaGitHub/coursework_drf.git

2. Создать виртуальное окружение:
  В терминале запустить команды:

    python -m venv venv
    source venv/bin/activate

3. Установить зависимости:
  Для установки всех зависимостей в терминале необходимо запустить команду:

    pip install -r requirements.txt

4. Cоздать базу данных:
  В терминале введите команду:

    CREATE DATABASE database_name

5. Применить миграции:
  В терминале введите команды:

    python3 manage.py makemigrations 
    python3 manage.py migrate

6. Заполнить файл .env по образцу .env.sample
7. Для создания суперпользователя необходимо применить команду:
    python3 manage.py csu
8. Для запуска проекта использовать команду: 
    python manage.py runserver
9. Для подключения бота в Телеграм перейти по ссылке:
    t.me/user_habit_bot
10. Для запуска периодических задач необходимо применить команду: 
    "celery -A config worker --beat --scheduler django --loglevel=info "
11. Документация API:
    Swagger http://127.0.0.1:8000/swagger/
    Redoc http://127.0.0.1:8000/redoc/

Инструкция для запуска проекта на удалённом сервере с помощью Docker:
1. Клонировать проект:
  https://github.com/jekaGitHub/coursework_drf.git
2. Переименовать файл .env.sample в .env и заполнить его необходимыми переменными
3. Ввести в терминале команду "docker-compose up -d --build"
Автор проекта: Евгений Сафонов
