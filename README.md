Yacut - сервис для укорачивания ссылок.

Клонировать репозиторий и перейти в него в командной строке:

```
git clone 
```

```
cd yacut
```

Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
```

* Если у вас Linux/macOS

    ```
    source venv/bin/activate
    ```

* Если у вас windows

    ```
    source venv/scripts/activate
    ```

Установить зависимости из файла requirements.txt:

```
python3 -m pip install --upgrade pip
```

```
pip install -r requirements.txt
```

Создать файл «.env», добавив в него переменные окружения:

```
touch.env
```

Выполнить команду запуска проекта:

```
flask run
```

Описание шаблона .env
Необходимо указать переменные окружения в следующем формате:

FLASK_APP = название приложения
FLASK_ENV = режим работы приложения: продакшен или разработка
DATABASE_URI = подключение БД, например: sqlite:///db.sqlite3
SECRET_KEY = уникальный секретный ключ