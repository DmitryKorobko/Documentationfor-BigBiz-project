Детальная информация о товаре
==============================

`GET /api/v1/product/detail?shop_id=..&id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/product/detail?shop_id=14&id=20`
-----------------------------------------------------------

```json
{
  "id": "1",
  "name": "Товар 1",
  "description": "<p>лучший</p>",
  "image": "/admin/images/uploads/user-3/product/DvRWD0bAohVWLv7wchlhb5uIACsXDGoe.jpeg",
  "availability": "1",
  "created_at": "1486988876",
  "prices": [
    {
      "id": "1",
      "product_id": "1",
      "count": "1",
      "price": "10"
    },
    {
      "id": "2",
      "product_id": "1",
      "count": "от 10",
      "price": "6"
    }
  ],
  "cities": [
    {
      "id": "1",
      "name": "Харьков"
    },
    {
      "id": "2",
      "name": "Киев"
    }
  ],
  "is_favorite": true,
  "count_reports": "2",
  "average_rating": "4.0000"
}
```