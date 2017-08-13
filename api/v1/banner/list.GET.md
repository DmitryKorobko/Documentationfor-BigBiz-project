Список активных баннеров
===============================

`GET /api/v1/banner/list`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа
-------------

```json
[
  {
    "id": "4",
    "image": "/admin/images/uploads/user-3/mobile_banner/oGgwph7Ftfkw0Ze0wQPvRpQ8yI5XSYRb.jpg"
  },
  {
    "id": "8",
    "image": "/admin/images/uploads/user-5/mobile_banner/dhyq7xMxDMq8cTzRmWVSuHZG-mZXOD-_.jpg"
  }
]
```