Отправление личного сообщения
==========================================

`POST /api/v1/message`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| recipient_id       | integer              | Идентификатор получателя           | +              |
| text               | string               | Текст сообщения                    | +              |
| images             | array                | Атрибуты картинки                  | -              |

Пример запроса `POST /api/v1/message`
----------------------------------------------------------
```json
{
    "text": "new message",
    "recipient_id": 2,
    "images": [
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNdN97d2PelAf9.png",
          "sort": 1
        },
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeHsdfsdfgcYQNdN97d2lAf9.png",
          "sort": 3
        } ,
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VozgcYQNddfghd2PelAf9.png",
          "sort": 2
        },
        {
          "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/message_images/9oyf_ahbHeH7VasdfsdfDFdN9d2PelAf9.png",
          "sort": 1
        }
    ]
}
```

Пример ответа `POST /api/v1/message`
------------------------------------------------------

```json
{
    "status": 200,
    "message": "Сообщение успешно отправлено",
    "data": {
        "id": 15,
        "created_by": 3,
        "recipient_id": 2,
        "text": "Hello!",
        "status": "UNREAD",
        "created_at": 1500296593,
        "updated_at": 1500296593,
        "images": [
            {
                "id": 6,
                "src": "https://s3-us-west-2.amazonaws.com/bigbiz/message_images/message-41/rgr3f_ahbsdfasdozgcYQNdN97d2Pelgf6.png"
            },
            {
                "id": 7,
                "src": "https://s3-us-west-2.amazonaws.com/bigbiz/message_images/message-41/rgr3f_ahbsdfasdozgcYQNdN97d2Pelgf6.png"
            }
        ]
    }
}
```