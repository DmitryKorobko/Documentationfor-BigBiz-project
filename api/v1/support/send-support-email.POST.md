Отправка письма в поддержку
========================

`POST /api/v1/support/send-letter`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание         | Обязательность |
|--------------------|----------------------|------------------|----------------|
| cause_send         | ENUM(                | Причина отправки | +              |
|                    |  APPLICATION_PROBLEM |                  |                |
|                    |  FUNCTIONAL_PROBLEM  |                  |                |
|                    |  WISHES              |                  |                |
|                    |)                     |                  |                |
|message             |text                  | Сообщение        | +              |

Пример ответа `POST /api/v1/support/send-letter`
---------------------

```json
{
    "status": 201,
    "message": "Письмо успешно отправлено",
    "data": {
        "id": 9,
        "user_id": 3,
        "name": "Website banner",
        "created_at": 1500295344,
        "updated_at": 1500295344,
        "cause_send": "WISHES",
        "message": "Admin! Where my website banner?",
        "status": "UNREAD"
    }
}
```