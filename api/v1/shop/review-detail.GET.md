Детальная информация об отзыве магазина оставленный конкретным пользователем
=======================================================

`GET /api/v1/shop/review-detail?shop_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/shop/review-detail?shop_id=11`
-----------------------------------------------------------

```json
{
  "id": 37,
  "shop_id": 11,
  "created_by": 9,
  "product_rating": 5,
  "operator_rating": 5,
  "reliability_rating": 4,
  "marker_rating": 4,
  "average_rating": 4.5,
  "created_at": 1491893188,
  "updated_at": 1491988013
}
```