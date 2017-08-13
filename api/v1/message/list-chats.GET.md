Список чатов
==============================

`GET /api/v1/message/list-chats`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/message/list-chats`
-------------------------------------------------------

```json
{
  "items": [
    {
      "recipient": {
        "name": "MariaFisher",
        "avatar": "/admin/images/uploads/user-5/profile/ZNMEANmWKpXfa3qQVTK8KmCM23_QPK27.jpg",
        "status_online": 1
      },
      "last_message": {
         "id": "9",
         "text": "new message 2",
         "recipient_id": 5,
         "created_at": 1488551045
      },
      "count_new_messages": 0
    },
    {
      "recipient": {
        "name": "MariaFisher",
        "avatar": "/admin/images/uploads/user-5/profile/ZNMEANmWKpXfa3qQVTK8KmCM23_QPK27.jpg",
        "status_online": 1
      },
      "last_message": {
        "id": 9,
        "text": "new message 2",
        "recipient_id": "5",
        "created_at": 1488551045
      },
      "count_new_messages": 2
    }
  ],
  "_links": {
          "self": {
              "href": "http://test.local/api/v1/message/list-chats?page=1&per-page=10"
          }
      },
      "_meta": {
          "totalCount": 2,
          "pageCount": 1,
          "currentPage": 1,
          "perPage": 10
      }
}
```