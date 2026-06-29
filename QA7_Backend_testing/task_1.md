# Задание 1. REST API

## Что такое REST API

REST API — это архитектурный стиль взаимодействия между клиентом и сервером через HTTP-запросы.

### Основные HTTP-методы

| Метод | Назначение |
|---|---|
| GET | Получение данных |
| POST | Создание данных |
| PUT | Полное обновление данных |
| PATCH | Частичное обновление данных |
| DELETE | Удаление данных |

---

## JSON

JSON (JavaScript Object Notation) — формат обмена данными между клиентом и сервером.

### Преимущества JSON перед XML

- Более компактный формат
- Проще читается
- Меньший размер данных
- Быстрее обрабатывается
- Удобен для JavaScript

### Отличия JSON от YAML

| JSON | YAML |
|---|---|
| Строгий синтаксис | Более читаемый |
| Используются скобки | Используются отступы |
| Часто используется в API | Часто используется в конфигурациях |

---

## JSON Schema

JSON Schema — это описание структуры JSON-документа:
- типы данных
- обязательные поля
- ограничения значений

---

## Сериализация и десериализация

- Сериализация — преобразование объекта в JSON
- Десериализация — преобразование JSON в объект

---

# Сравнение REST API

## Выбранные API

1. JSONPlaceholder  
https://jsonplaceholder.typicode.com

2. ReqRes  
https://reqres.in

---

## Сравнительная таблица API

| Критерий | JSONPlaceholder | ReqRes |
|---|---|---|
| Документация | https://jsonplaceholder.typicode.com | https://reqres.in |
| Основные методы | GET, POST, PUT, PATCH, DELETE | GET, POST, PUT, DELETE |
| Формат запросов | JSON | JSON |
| Формат ответов | JSON | JSON |
| Авторизация | Не требуется | API Key |
| Версия API | Не указана | v1 |
| Назначение | Тестовый fake API | API для тестирования запросов и авторизации |
| Структура API | Простая и минималистичная | Более приближена к реальному сервису |

---

# Основные эндпоинты

## JSONPlaceholder

| Endpoint | Метод |
|---|---|
| /posts | GET |
| /posts/1 | GET |
| /posts | POST |
| /posts/1 | PUT |
| /posts/1 | PATCH |
| /posts/1 | DELETE |

---

## ReqRes

| Endpoint | Метод |
|---|---|
| /api/users | GET |
| /api/users/2 | GET |
| /api/users | POST |
| /api/login | POST |
| /api/users/2 | PUT |
| /api/users/2 | DELETE |

# Пример JSON-ответа

Выбранный API: JSONPlaceholder

Ссылка на API:  
https://jsonplaceholder.typicode.com/posts/1

## Пример ответа

```json
{
  "userId": 1,
  "id": 1,
  "title": "sunt aut facere repellat provident occaecati",
  "body": "quia et suscipit suscipit recusandae"
}
```

---

# Анализ структуры JSON

| Ключ | Тип данных | Описание |
|---|---|---|
| userId | Number | ID пользователя |
| id | Number | ID записи |
| title | String | Заголовок поста |
| body | String | Текст поста |