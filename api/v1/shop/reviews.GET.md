Список отзывов о магазине
=========================
   
`GET /api/v1/shop/reviews?shop_id=...`
   
## Принимаемые заголовки
   
| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |
   
   
Пример ответа `GET /api/v1/shop/reviews?shop_id=8`
--------------------------------------------------
   
```json
{
  "items": [
    {
      "id": 4,
      "product_rating": 5,
      "operator_rating": 5,
      "reliability_rating": 5,
      "marker_rating": 5,
      "average_rating": 5,
      "created_at": 1491381790,
      "created_by": {
        "name": "Batman",
        "avatar": "/admin/images/uploads/user-4/profile/EQuMJklURdfK2uIcztJB6L4GePqLNzzK.jpg",
        "is_online": true
      }
    },
    {
      "id": 62,
      "product_rating": 5,
      "operator_rating": 5,
      "reliability_rating": 5,
      "marker_rating": 4,
      "average_rating": 4.75,
      "created_at": 1492602482,
      "created_by": {
        "name": "bbuserbb",
        "avatar": null,
        "is_online": false
      }
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/shop/reviews?shop_id=8&page=1&per-page=10"
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