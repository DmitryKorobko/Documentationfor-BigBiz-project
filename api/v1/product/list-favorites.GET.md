Список продуктов в избранном
==============================

`GET /api/v1/product/list-favorites`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/product/list-favorites`
-------------------------------------------------------

```json
{
  "items": [
    {
      "id": 1,
      "name": "Колесо переднее",
      "image": "/admin/images/uploads/user-8/product/XOc47FcTyaU3PMp9y_qZlLO3JXrSS5V4.jpg",
      "average_rating": 5.0000,
      "count_report": 2,
      "availability": "Есть в наличии",
      "price": 1500
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/user/product/list-favorites?page=1&per-page=10"
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