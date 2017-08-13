Выход пользователя
========================

`GET /api/v1/authorization/logout`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Пример ответа `GET /api/v1/authorization/logout`

```json
{
    "status": 200,
    "code": 15,
    "message": "Сессия успешно закрыта."
}
```