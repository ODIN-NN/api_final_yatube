# api_final

Учебный проект Api_final предстовляет собой набор функций 
для получения, добавления и редактирования информации но портале Yatube.
# Как запустить проект:
Клонировать репозиторий:

```
git clone https://github.com/ODIN-NN/api_final_yatube.git
```

Перейти в директорию с помощью командной строки:

```
cd api_final_yatube
```

Cоздать и активировать виртуальное окружение:

```
python -m venv env
```

```
source venv/Scripts/activate
```

Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Выполнить миграции:

```
python manage.py migrate
```

Запустить проект:

```
python manage.py runserver
```
 # Примеры запросов и ответов
 POST запрос к эндпоинту http://127.0.0.1:8000/api/v1/posts/    
 с данными 
{
    "text": "Just text"
}
создаст пост с заданными данными   
 ____
 GET запрос к эндпоинту http://127.0.0.1:8000/api/v1/posts/    
 вернёт список всех постов. Ответ будет выглядеть следующим образом:    
 ```python
 [
    {
        "id": 1,
        "author": "alex",
        "text": "Just text",
        "pub_date": "2022-09-29T12:37:41.789918Z",
        "image": null,
        "group": null
    }
]
```