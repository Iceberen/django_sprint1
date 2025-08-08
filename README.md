# 📰 Blogicum — Django Sprint 1

Учебный проект, реализующий блог-платформу с помощью Django.  
Репозиторий создан в рамках первого спринта по курсу Backend-разработки.

---

## 📌 Описание

**Blogicum** — это простой новостной сайт, где реализованы базовые функции:
- Главная страница со списком публикаций
- Страницы с деталями каждой публикации
- Категории новостей и фильтрация по ним
- Статические страницы: "О проекте" и "Правила"

Все данные о публикациях представлены в виде статического списка в коде (без подключения БД).

---

## 🧱 Стек технологий

- Python 3.10+
- Django 4.x
- HTML + шаблоны Django
- CSS (Bootstrap)
- Pytest (для автотестов)

---

## 🚀 Установка и запуск

1. Клонируйте репозиторий:
    ```
    git clone https://github.com/Iceberen/django_sprint1.git
    cd django_sprint1/blogicum

2. Cоздать и активировать виртуальное окружение:
    ```
    python -m venv venv
    source venv/bin/activate     # для Linux/macOS
    venv\Scripts\activate        # для Windows

3. Установить зависимости из файла requirements.txt:
    ```
    pip install -r requirements.txt

4. Запустите сервер:
    ```
    python3 manage.py runserver     # для Linux/macOS
    python manage.py runserver      # для Windows

5. Откройте в браузере:
    http://127.0.0.1:8000/

---

## 🗺 Структура проекта
```
blogicum/
├── blog/
│   ├── views.py — логика отображения постов и категорий
│   ├── urls.py — маршруты для постов
│   └── templates/blog/ — шаблоны для списка, категорий, деталей
│
├── pages/
│   ├── views.py — отображение статических страниц
│   └── templates/pages/ — about.html, rules.html
│
├── static_dev/
│   ├── css/ — Bootstrap стили
│   └── img/ — изображения (логотип, фавиконы)
│
├── templates/
│   └── base.html — базовый шаблон
│
├── blogicum/ — настройки Django-проекта
│   ├── settings.py
│   ├── urls.py
│   └── wsgi.py, asgi.py
│
├── manage.py
```

---

## 🧪 Тестирование
Тесты находятся в директории tests/.
Для запуска:
```
pytest
```

---

## 👤 Автор
Разработано: [Iceberen](https://github.com/Iceberen) в рамках учебного спринта по Django.