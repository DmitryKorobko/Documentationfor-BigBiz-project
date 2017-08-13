Список тем магазина
===================
   
`GET /api/v1/theme/shop-themes?shop_id=...`
   
## Принимаемые заголовки
   
| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |
   
   
Пример ответа `GET /api/v1/theme/shop-themes?shop_id=8`
--------------------------------------------------
   
```json
{
  "items": [
    {
      "id": 4,
      "category_name": "Экстрим",
      "name": "Даунхилл",
      "shop_name": "Velo Mag",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1492691714,
      "count_like": 1,
      "count_dislike": 0,
      "is_favorite": false,
      "is_like": 0,
      "is_dislike": 0
    },
    {
      "id": 10,
      "category_name": "Похудение",
      "name": "Скакалка",
      "shop_name": "Velo Mag",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1496918269,
      "count_like": 2,
      "count_dislike": 0,
      "is_favorite": false,
      "is_like": 1,
      "is_dislike": 0
    },
    {
      "id": 2,
      "category_name": "Похудение",
      "name": "Велопрогулка",
      "shop_name": "Velo Mag",
      "view_count": 2,
      "comments_count": 0,
      "date_of_publication": 1492691715,
      "count_like": 2,
      "count_dislike": 0,
      "is_favorite": false,
      "is_like": 0,
      "is_dislike": 0
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/theme/shop-themes?shop_id=8&page=1&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 3,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 10
  }
}
```