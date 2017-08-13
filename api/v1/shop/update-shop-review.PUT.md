Обновить отзыв о магазине
=============================

`PUT /api/v1/shop/update-shop-review`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| shop_id            | integer              | Магазин                                       | +              |
| product_rating     | integer              | Качество товара                               | +              |
| operator_rating    | integer              | Качество работы оператра                      | +              |
| reliability_rating | integer              | Надежность магазина                           | +              |
| marker_rating      | integer              | Качество доставки                             | +              |

Пример ответа `PUT /api/v1/shop/update-shop-review`
----------------------------------------

```json
{
  "status": 200,
  "message": "Отзыв о магазине успешно изменён",
  "data": {
      "id": 2,
      "shop_id": 3,
      "created_by": 3,
      "product_rating": 2,
      "operator_rating": 1,
      "reliability_rating": 1,
      "marker_rating": 1,
      "average_rating": 1.25,
      "created_at": 1500291716,
      "updated_at": 1500292237,
      "status": "UNREAD"
  }
}
```