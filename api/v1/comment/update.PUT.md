Обновление комментария
=============================

`PUT /api/v1/comment`

## Принимаемые заголовки

| Название                   | Значение                        | Обязательность                       |
|----------------------------|---------------------------------|--------------------------------------|
| Content-Type               | application/json                | +                                    |
| Authorization              | Bearer auth_token               | +                                    |

## Принимаемые поля

| Поле               | Тип                  | Описание          | Обязательность |
|--------------------|----------------------|-------------------|----------------|
| text               | text                 | Текст комментария | +              |
| theme_id           | integer              | ID темы           | +              |
| comment_id         | integer              | ID комментария    | +              |
| recipient_id       | integer              | ID получателя     | -              |
| images             | array                | Атрибуты картинки | -              |

Пример запроса `PUT /api/v1/comment`
----------------------------------------------------------

```json
{
    "text": "comment comment",
    "theme_id": 1,
    "comment_id": 41,
    "images": {
        "delete": [
            {
              "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozgcYQNdN97d2Pelyf3.png"
            },
            {
              "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozycYQNeN97dffelyf5.png"
            }
        ],
        "create": [
            {
                "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbsdfasdozgcYQNdN97d2Pelgf6.png",
                "sort": 1
            },
            {
                "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozgcsdtggN97d2Pelof8.png",
                "sort": 2
            }
        ]
    }
}

```
Пример ответа `PUT /api/v1/comment`
----------------------------------------

```json
{
    "status": 200,
    "message": "Комментарий успешно изменён",
    "data": {
        "id": 7,
        "text": "какой-то комментарий",
        "theme_id": 1,
        "created_by": 3,
        "recipient_id": 2,
        "status": "UNREAD",
        "created_at": 1497601030,
        "updated_at": 1497601043,
        "images": {
            "created": [
                {
                    "id": 2,
                    "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbsdfasdozgcYQNdN97d2Pelgf6.png"
                },
                {
                    "id": 3,
                    "src": "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozgcsdtggN97d2Pelof8.png"
                }
            ]
        }
    }
}
```
