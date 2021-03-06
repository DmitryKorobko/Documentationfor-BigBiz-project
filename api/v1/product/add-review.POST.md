Добавление отзыва о товаре
==============================

`POST /api/v1/product/add-review`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| product_id         | integer              | id товара                          | +              |
| rating             | integer              | Рейтинг товара                     | +              |
| text               | text                 | Отзыв о товаре                     | +              |


Пример ответа `POST /api/v1/product/add-review`
------------------------------------------------------

```json
{
    "status": 201,
    "message": "Отзыв успешно добавлен",
    "data": {
        "id": 3,
        "text": "good product",
        "product_id": 1,
        "user_id": 3,
        "rating": 7,
        "created_at": 1500293229,
        "updated_at": 1500293229
    }
}
```