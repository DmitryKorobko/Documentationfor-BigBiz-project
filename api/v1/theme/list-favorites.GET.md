Список тем в избранном
==============================

`GET /api/v1/theme/list-favorites`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/theme/list-favorites`
-----------------------------------------------------------

```json
{
  "items": [
    {
      "name": "Правильное питание",
      "category_name": "Похудение",
      "view_count": 2,
      "comments_count": 0,
      "date_of_publication": 1490956387,
      "count_like": 2,
      "count_dislike": 1,
      "is_like": 1,
      "is_dislike": 0,
      "user_name": "Witcher"
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/theme/list-favorites?page=1&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 1,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 10
  }
}
```