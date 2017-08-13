Список комментариев темы
==============================

`GET /api/v1/comment/list?theme_id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание       | Обязательность |
|--------------------|----------------------|----------------|----------------|
| theme_id           | integer              | ID темы        | +              |

Пример ответа `GET /api/v1/comment/list?theme_id=1`
--------------------------------------------------
   
```json
{
    "items": [
        {
            "recipient": {
                "id": 1,
                "name": "guest"
            },
            "author": {
                "id": "1",
                "name": "guest",
                "avatar": null,
                "status_online": 1
            },
            "comment": {
                "id": "2",
                "text": "естественно возрастающий минимум",
                "created_at": "1495533616",
                "status": "UNREAD",
                "count_like": "3",
                "liked": true,
                "images": [
                    {
                        "src": "image.jpeg"
                    }
                ]
            }
        },
        {
            "recipient": {
                "id": 1,
                "name": "guest"
            },
            "author": {
                "id": "1",
                "name": "guest",
                "avatar": null,
                "status_online": 1
            },
            "comment": {
                "id": "5",
                "text": "голова чтобы думать, ноги чтобы ходить",
                "created_at": "1497340137",
                "status": "UNREAD",
                "count_like": "0",
                "liked": false,
                "images": []
            }
        }
    ],
    "_links": {
        "self": {
            "href": "http://test.local/api/v1/comment/list?theme_id=1&page=1&per-page=10"
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