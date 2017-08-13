Список собственных тем пользователя
===================================

`GET /api/v1/user/theme`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET GET /api/v1/user/theme`
-------------

```json
{
  "items": [
    {
      "id": 3,
      "name": "Правильное питание",
      "view_count": 2,
      "status": "VERIFIED",
      "image": null,
      "category_name": "Похудение",
      "category_id": 1,
      "comments_count": 0,
      "date_of_publication": 1490956387,
      "count_like": 1,
      "count_dislike": 1
    },
    {
      "id": 5,
      "name": "Зарядка",
      "view_count": 0,
      "status": "UNVERIFIED",
      "image": null,
      "category_name": "Похудение",
      "category_id": 1,
      "comments_count": 0,
      "date_of_publication": 1492690801,
      "count_like": 0,
      "count_dislike": 0
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/user/theme/index?page=1&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 2,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 10
  }
}
```