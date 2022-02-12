### Что же это за проект?

В этом проекте можно писать и получать посты и подписываться на интересных авторов.

Он создан с помощью API.

В этом проекте мои страдания, польза от него, что бы я научилась.

### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram2plus.git
```

```
cd kittygram2plus
```

Cоздать и активировать виртуальное окружение, а если у Вас PyCharm, то он сам все развернет:

```
python3 -m venv env
```

```
source env/bin/activate
```

```
python3 -m pip install --upgrade pip
```

Установить зависимости из файла requirements.txt:

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python3 manage.py migrate
```

Запустить проект:

```
python3 manage.py runserver
```

Примеры запросов

GET-запрос http://127.0.0.1:8000/api/v1/posts/

```
{
    "text": "string",
    "image": "string",
    "group": 0
}
```

POST-запрос http://127.0.0.1:8000/api/v1/posts/{id}/

```
{
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0
}
```

GET-запрос http://127.0.0.1:8000/api/v1/posts/{id}/

```
{
    "id": 0,
    "author": "string",
    "text": "string",
    "pub_date": "2019-08-24T14:15:22Z",
    "image": "string",
    "group": 0
}
```

GET-запрос http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/

```
{
    "id": 0,
    "author": "string",
    "text": "string",
    "created": "2019-08-24T14:15:22Z",
    "post": 0
}
```

POST-запрос http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/

```
{
    "text": "string"
}
```

GET-запрос http://127.0.0.1:8000/api/v1/posts/{post_id}/comments/{id}/

```
{
    "id": 0,
    "author": "string",
    "text": "string",
    "created": "2019-08-24T14:15:22Z",
    "post": 0
}
```


GET-запрос http://127.0.0.1:8000/api/v1/groups/

```
{
    "id": 0,
    "title": "string",
    "slug": "string",
    "description": "string"
}
```

GET-запрос http://127.0.0.1:8000/api/v1/groups/

```
{
    "id": 0,
    "title": "string",
    "slug": "string",
    "description": "string"
}
```

GET-запрос http://127.0.0.1:8000/api/v1/groups/{id}/

```
{
    "id": 0,
    "title": "string",
    "slug": "string",
    "description": "string"
}
```

GET-запрос http://127.0.0.1:8000/api/v1/follow/

```
{
    "user": "string",
    "following": "string"
}
```

POST-запрос http://127.0.0.1:8000/api/v1/follow/

```
{
    "user": "string",
    "following": "string"
}
```

