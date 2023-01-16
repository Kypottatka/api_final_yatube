# api_final
api final

### Описание проекта
API для проекта Yatube, социальной медиа платформы для обмена и поиска медиа.


### Как запустить проект:

Клонировать репозиторий и перейти в него в командной строке:

```
git clone https://github.com/yandex-praktikum/kittygram.git
```

```
cd kittygram
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv env
```

```
source env/bin/activate
```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

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


### Endpoints
/api/v1/posts/: CRUD operations for posts
/api/v1/comments/: CRUD operations for comments
/api/v1/likes/: CRUD operations for likes
/api/v1/users/: CRUD operations for users


### Аутентфикация
Это API использует аутентифекацию на основе JWT токенов. Вы можете получить токен, сделав POST запрос на '/api/v1/token/', введя свои логин и пароль.


### Разрешения
- Пользователи могут редактировать и удалять только свои собственные посты, комментарии и подписки
- Неавторизованные пользователи могут только просматривать контент, за исключением подписок

### Разработано с использованием
- Django
- Django REST framework
- djangorestframework-jwt

### Лицензия
This project is licensed under the MIT License - see the LICENSE file for details.