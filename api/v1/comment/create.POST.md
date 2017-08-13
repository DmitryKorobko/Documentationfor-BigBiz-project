Добавление комментария
========================

`POST /api/v1/comment`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание          | Обязательность |
|--------------------|----------------------|-------------------|----------------|
| text               | text                 | Текст комментария | +              |
| theme_id           | integer              | ID темы           | +              |
| recipient_id       | integer              | ID получателя     | -              |
| images             | array                | Атрибуты картинки | -              |

Пример запроса `POST /api/v1/comment`
----------------------------------------------------------
```json
{
    "text" : "comment",
    "theme_id" : 1,
    "recipient_id" : 2,
    "images" : [
        {
          "src" : "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozgcYQNdN97d2PelAf9.png",
          "sort" : 1
        },
        {
          "src" : "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeHsdfsdfgcYQNdN97d2lAf9.png",
          "sort" : 1
        } ,
        {
          "src" : "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VozgcYQNddfghd2PelAf9.png",
          "sort" : 2
        },
        {
          "src" : "http://assets-dev.ourcnc.com.s3.eu-central-1.amazonaws.com/comment_images/9oyf_ahbHeH7VasdfsdfDFdN9d2PelAf9.png",
          "sort" : 1
        }
    ]
}
```
Пример ответа `POST /api/v1/comment`
----------------------------------------------------------

```json
{
    "status": 201,
    "message": "Комментарий успешно добавлен",
    "data": {
        "id": 7,
        "text": "какой-то комментарий",
        "theme_id": 1,
        "created_by": 3,
        "recipient_id": 2,
        "status": "UNREAD",
        "created_at": 1497601030,
        "updated_at": 1497601043,
        "images": [
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
```