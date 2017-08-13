Изменение личного сообщения
==========================================

`PUT /api/v1/message/{id}`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| text               | string               | Текст сообщения                    | +              |
| recipient_id       | integer              | ID получателя                      | -              |
| images             | array                | Атрибуты картинки                  | -              |

Пример запроса `PUT /api/v1/message/7`
----------------------------------------------------------

```json
{
    "text" : "comment comment",
    "images" : {
        "delete" : [
            {
              "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN97d2Pelyf3.png"
            },
            {
              "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN97d2Pelyf3.png"
            }
        ],
        "create" : [
            {
                "src" : "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbsdfasdozgcYQNdN97d2Pelgf6.png",
                "sort" : 1
            },
            {
                "src" : "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcsdtggN97d2Pelof8.png",
                "sort" : 2
            }
        ]
    }
}

```

Пример ответа `PUT /api/v1/message/7`
------------------------------------------------------

```json
{
    "status": 200,
    "message": "Сообщение успешно изменено",
    "data": {
        "id": 7,
        "created_by": 6,
        "recipient_id": 5,
        "text": "new message!!!!!!!",
        "status": "READ",
        "created_at": 1488551030,
        "updated_at": 1488555209,
        "images": {
            "created": [
                {
                    "id": 12,
                    "src": "https://s3-us-west-2.amazonaws.com/bigbiz/message_images/message-7/9oyf_ahbsdfasdozgcYQNdN97d2Pelgf6.png"
                },
                {
                    "id": 13,
                    "src": "https://s3-us-west-2.amazonaws.com/bigbiz/message_images/message-7/9oyf_ahbHeH7VozgcsdtggN97d2Pelof8.png"
                }
            ]
        }
    }
}
```