Список ответов для магазина
===========================
   
`GET /api/v1/shop/answers?status=...`
   
## Принимаемые заголовки
   
| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |
   
## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| status             | READ|UNREAD          | Статус ответа                                 | +              |
   
   
Пример ответа `GET /api/v1/shop/answers?status=UNREAD`
--------------------------------------------------
   
```json
{
  "items": [
    {
      "id": 6,
      "type": "LIKE_THEME",
      "product_id": 3,
      "theme_id": 4,
      "comment_id": 2,
      "created_at": 1492525792,
      "text": "оценил вашу тему",
      "status": "UNREAD",
      "created_by": {
        "user_name": "bbuserbb",
        "user_image": "/admin/images/uploads/user-9/profile/witcher.png",
        "is_online": false
      }
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/shop/answers?status=UNREAD&page=1&per-page=10"
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