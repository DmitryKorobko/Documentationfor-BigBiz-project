Список ответов для пользователя
===============================
   
`GET /api/v1/user/profile/answers?status=...`
   
## Принимаемые заголовки
   
| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |
   
## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| status             | READ|UNREAD          | Статус ответа                                 | +              |
   
Пример ответа `GET /api/v1/user/profile/answers?status=UNREAD`
--------------------------------------------------
   
```json
{
  "items": [
    {
      "id": 12,
      "type": "LIKE_THEME",
      "product_id": 2,
      "theme_id": 7,
      "comment_id": 3,
      "created_at": 1492784190,
      "text": "Оценил вашу тему",
      "status": "UNREAD",
      "created_by": {
        "user_name": "bbuserbb",
        "user_image": "/admin/images/uploads/user-9/profile/witcher.png",
        "is_online": false
      }
    },
    {
      "id": 11,
      "type": "LIKE_THEME",
      "created_at": 1492784190,
      "text": "Оценил вашу тему",
      "status": "UNREAD",
      "created_by": {
        "user_name": "bbuserbb",
        "user_image": "/admin/images/uploads/user-11/profile/witcher.png",
        "is_online": false
      }
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/user/answers?status=UNREAD&page=1&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 1,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 10
  }
}
```