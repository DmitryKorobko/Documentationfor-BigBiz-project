Настройка таймера очищения истории
==========================================

`POST /api/v1/message/cleaning-chat`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле                       | Тип                             | Описание                             | Обязательность |
|----------------------------|---------------------------------|--------------------------------------|----------------|
| frequency_history_cleaning | ENUM('ONE_MINUTE',              | Частота очистки истории сообщений    | +              |
|                            |    'FIVE_MINUTES', 'ONE_HOUR',  |                                      |                |
|                            |    'THREE_HOURS', 'FIVE_HOURS', |                                      |                |
|                            |    'TWELVE_HOURS', 'ONE_DAY',   |                                      |                |
|                            |    'SEVEN_DAYS','NEVER)         |                                      |                |

Пример ответа `PUT /api/v1/message/cleaning-chat`
-------------------------------------------------

```json
{
    "status": 200,
    "message": "Таймер очистки личных сообщений успешно настроен",
    "data": {
        "id": 11,
        "user_id": 58,
        "show_date_of_birth": 1,
        "show_status_online": 1,
        "view_page_access": "ALL_USERS",
        "send_messages_access": "ALL_USERS",
        "frequency_history_cleaning": "ONE_MINUTE",
        "created_at": 1497528631,
        "updated_at": 1500036689
    }
}
```