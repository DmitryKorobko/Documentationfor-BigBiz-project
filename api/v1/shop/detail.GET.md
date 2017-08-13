Детальная информация о магазине
===============================

`GET /api/v1/shop/detail?shop_id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/shop/detail?shop_id=11`
-----------------------------------------------------------

```json
{
  "id": 9,
  "name": "Velo Style",
  "status_text": "Our company - is many mountain bikes",
  "image": "/admin/images/uploads/user-11/profile/I9PY7miPzqrYPJyJoCzgqH8bLk1b5jiM.jpg",
  "user_id": 11,
  "work_start_time": "10:00",
  "work_end_time": "20:00",
  "skype": "vsSky",
  "viber": "vsVib",
  "telegram": "vsTel",
  "jabber": "vsJab",
  "vipole": "vsVip",
  "user_registration_date": 1491466583,
  "rating": 4.9,
  "count_themes": 0,
  "count_products": 0,
  "count_reviews": 2,
  "is_online": false,
  "cities": [
    {
      "id": 3,
      "name": "Киев"
    },
    {
      "id": 4,
      "name": "Харьков"
    },
    {
      "id": 5,
      "name": "Одесса"
    },
    {
      "id": 8,
      "name": "Львов"
    }
  ]
}
```