История сообщений конкретного чата
===================================

`GET /api/v1/message/history-chat?recipient_id=......`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/message/history-chat?recipient_id=5`
-------------------------------------------------------

```json
{
  "items": [
    {
      "id": 9,
      "text": "new message 2",
      "status": "READ",
      "created_at": 1488551045,
      "images": [
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN97d2PelAf9.png"
        },
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN97d2PelAf9.png"
        }
      ]
    },
    {
      "id": 8,
      "text": "new message 1",
      "status": "READ",
      "created_at": 1488551040,
      "images": []
    },
    {
      "id": 7,
      "text": "new message!!!!!!!",
      "status": "READ",
      "created_at": 1488551030,
      "images": [
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN9sdfsdfsdf.png"
        },
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN9asdffdTTE.png"
        }
      ]
    }
  ],
  "_links": {
    "self": {
      "href": "http://api/v1/message/history-chat?recipient_id=5&page=1"
    }
  },
  "_meta": {
    "totalCount": 3,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 20
  }
}
```