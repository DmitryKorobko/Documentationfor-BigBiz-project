Обновить отзыв о товаре
=============================

`PUT /api/v1/product/update-review`

## Принимаемые заголовки

| Название                   | Значение                        | Обязательность                       |
|----------------------------|---------------------------------|--------------------------------------|
| Content-Type               | application/json                | +                                    |
| Authorization              | Bearer auth_token               | +                                    |

## Принимаемые поля

| Поле                       | Тип                             | Описание                             | Обязательность |
|----------------------------|---------------------------------|--------------------------------------|----------------|
| product_id                 | integer                         | ID товара                            | +              |
| review_id                  | integer                         | ID отзыва                            | +              |
| text                       | text                            | Отзыв о товаре                       | +              |
| rating                     | integer                         | Рейтинг товара                       | +              |

Пример ответа `PUT /api/v1/product/update-review`
----------------------------------------

```json
{
  "status": 200,
  "message": "Отзыв товара успешно изменён",
  "data": {
      "id": 3,
      "text": "very good product",
      "product_id": 1,
      "user_id": 3,
      "rating": 7,
      "created_at": 1500293229,
      "updated_at": 1500293229
  }
}
```