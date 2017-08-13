Детальная информация о магазине
===============================

`GET /api/v1/shop/profile`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/shop/profile`
-----------------------------------------------------------

```json
{
  "id": 8,
  "name": "Velo Mag",
  "status_text": "Our shop - it's the best bikes!",
  "image": "/admin/images/uploads/user-8/profile/b7chYJ8exD07m3F0jyzj7MpvSP-hZcLu.jpg",
  "user_id": 8,
  "user_registration_date": 1490940211,
  "work_start_time": "09:00",
  "work_end_time": "18:00",
  "skype": "velomagSky",
  "viber": "velomagVib",
  "telegram": "velomagTel",
  "jabber": "velomagJab",
  "vipole": "velomagVip",
  "rating": 4.5,
  "count_themes": 2,
  "count_products": 3,
  "count_reviews": 1,
  "is_online": false
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
    }
  ]
}
```