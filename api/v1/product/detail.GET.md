Детальная информация о продукте
===============================

`GET /api/v1/product/detail?id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/product/detail?id=1
-----------------------------------------------------------

```json
{
  "id": 1,
  "name": "frame",
  "description": "A bicycle frame is the main part of the bicycle to which the bicycle components are attached",
  "image": "/admin/images/uploads/user-11/profile/I9PY7miPzqrYPJyJoCzgqH8bLk1b5jiM.jpg",
  "availability": 1,
  "created_at": 1234234,
  "updated_at": 2342144,
  "user_id": 1,
  "is_favorite": false,
  "count_reports": 0,
  "average_rating": 0,
  "prices": [
    {
      "id": 1,
      "product_id": 1,
      "count": 3,
      "price": 123
    }
  ],
  "cities": [
    {
      "id": 1,
      "name": "Киев"
    }
  ]
}