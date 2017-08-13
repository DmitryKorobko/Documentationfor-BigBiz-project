Удаление истории сообщений с конкретным пользователем
=====================================================

`DELETE /api/v1/message/delete-chat?recipient_id=......`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## пример ответа `DELETE /api/v1/message/delete-chat?recipient_id=3`

```json
{
  "status": 200,
  "message": "Чат с пользователем успешно удалён"
}
```