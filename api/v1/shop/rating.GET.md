Полная информация о рейтинге магазина
===================================================

`GET /api/v1/shop/rating?shop_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/shop/rating?shop_id=14`
--------------------------------------------------

```json
{
  "shop_name": "Candy Shop",
  "avatar": "/admin/images/uploads/user-3/profile/AFCscI-l8oC9iCs7denWDBuzXolCbRK3.jpg",
  "rating": {
    "average_product_rating": 3,
    "average_reliability_rating": 3.5,
    "average_operator_rating": 3,
    "average_marker_rating": 4,
    "average_rating": 3.4
  }
}
```