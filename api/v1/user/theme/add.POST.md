Добавление собственной темы пользователем
==========================================

`POST /api/v1/user/theme/create`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| category_id        | integer              | Категория темы                     | +              |
| name               | string               | Название темы                      | +              |
| description        | string               | Контент темы                       | +              |

Пример ответа `POST /api/v1/user/theme/create`
------------------------------------------------------

```json
{
    "status": 201,
    "message": "Тема успешно создана",
    "data": {
        "id": 4,
        "name": "new theme",
        "description": "super theme",
        "image": null,
        "view_count": 2,
        "comments_count": 2,
        "new_comments_count": 1,
        "user_id": 3,
        "category_id": 2,
        "date_of_publication": 1500283401,
        "sort": 1,
        "status": "UNVERIFIED",
        "created_at": 1500283401,
        "updated_at": 1500283401
    }
}
```
