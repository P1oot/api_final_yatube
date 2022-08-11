# api_final

## Описание.

Проект представляет из себя социальную сеть на основе API запросов.
С его помощью можно создавать посты, оставлять комментарии и подписываться на других пользователей.

## Установка.

Клонировать репозиторий и перейти в него в командной строке:
`git clone git@github.com:P1oot/api_final_yatube.git`
`cd api_final_yatube`

Cоздать и активировать виртуальное окружение:
`python -m venv env`
`source env/bin/activate`

Установить зависимости из файла requirements.txt:
`python -m pip install --upgrade pip`
`pip install -r requirements.txt`

Выполнить миграции:
`python manage.py migrate`

Запустить проект:
`python manage.py runserver`

## Примеры запросов.

"Получение JWT токена":     "http://127.0.0.1:8000/api/v1/jwt/create/"
"Обращение к простам":      "http://127.0.0.1:8000/api/v1/posts/"
"Обращение к комментариям": "http://127.0.0.1:8000/api/v1/posts/{pk}/comments"
"Обращение к группам":      "http://127.0.0.1:8000/api/v1/groups/"
"Обращение к подпискам":    "http://127.0.0.1:8000/api/v1/follow/"
