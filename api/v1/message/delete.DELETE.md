Удаление сообщения
==============

`DELETE /api/v1/message/{id}`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Пример ответа `/api/v1/message/5`

```json
{
    "status": 200,
    "message": "Сообщение успешно удалёно",
    "data": {
        "message_id": 15
    }
}
```