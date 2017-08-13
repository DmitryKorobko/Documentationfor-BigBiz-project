Добавление отзывы о магазине пользователем
==============================

`POST /api/v1/shop/add-shop-review`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| product_rating     | integer              | Рейтинг качество продукта          | +              |
| operator_rating    | integer              | Рейтинг качество работы оператора  | +              |
| reliability_rating | integer              | Рейтинг надежности магазина        | +              |
| marker_rating      | integer              | Рейтинг доставки товара            | +              |
| shop_id            | integer              | Идентификатор магазина             | +              |

Пример ответа `POST /api/v1/shop/add-shop-review`
------------------------------------------------------

```json
{
    "status": 201,
    "message": "Отзыв о магазине успешно добавлен",
    "data": {
        "id": 2,
        "shop_id": 3,
        "created_by": 3,
        "product_rating": 1,
        "operator_rating": 1,
        "reliability_rating": 1,
        "marker_rating": 1,
        "average_rating": 1,
        "created_at": 1500291716,
        "updated_at": 1500291716,
        "status": "READ"
    }
}
```