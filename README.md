# What to watch
## Сервис, помогающий выбрать фильм для просмотра


## Описание
__What to watch__ позволяет:
* сформировать базу отзывов о фильмах
* облегчить выбор фильма для просмотра
Реализована работа сервиса как с использованием html-шаблонов, так и через api


## Технологии
* Python 3.11
* Flask 2.0.2
* Flask-SQLAlchemy 2.5.1
* SQLalchemy 1.4.49
* Alembic 1.12


## Как запустить проект

1. Клонировать репозиторий и перейти в него в командной строке:

```
git clone
```

2. Cоздать и активировать виртуальное окружение:

```
python3 -m venv venv
source venv/bin/activate
```

или для пользователей Windows

```
python -m venv venv
source venv/Scripts/activate
```

3. Установить зависимости из файла requirements.txt:

```
python -m pip install --upgrade pip
pip install -r requirements.txt
```

4. Создать файл .env и заполнить его переменными окружения и их значениями. Пример заполнения приведен в файле .env.example
5. Подготовить базу данных
* примените миграции
```
flask db upgrade
```
* для заполнения базы данных фильмами и отзывами из файла load_opinions.csv выполните команду
```
flask load_opinions
```

6. Запустить проект:

```
flask run
```
