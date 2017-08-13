Общий список избранных продуктов и тем
======================================

`GET /api/v1/user/common-list-favorites`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/user/common-list-favorites`
-------------------------------------------------------

```json
{
  "themes": [
    {
      "name": "1111",
      "category_name": "Новости",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1491310484,
      "count_like": 0,
      "count_dislike": 0,
      "user_name": "Администрация"
    }
  ],
  "products": [
    {
      "name": "Гашиш",
      "image": "/admin/images/uploads/user-3/product/DvRWD0bAohVWLv7wchlhb5uIACsXDGoe.jpeg",
      "average_rating": 4.0000,
      "count_report": 2,
      "availability": "Есть в наличии",
      "price": "10"
    },
    {
      "name": "шишки",
      "image": "/admin/images/uploads/user-5/product/jIfQ4u6ae5jz_JieT4FolXQdi2QUTPf0.jpg",
      "average_rating": 0,
      "count_report": 0,
      "availability": "Есть в наличии",
      "price": 250
    }
  ]
}
```