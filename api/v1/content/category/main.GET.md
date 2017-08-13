Список категорий первого уровня
===============================

`GET /api/v1/content/category/list-main`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа
-------------

```json
{
  "items": [
    {
      "id": 1,
      "name": "BigBiz",
      "sort": 1,
      "created_at": 1487066340,
      "updated_at": 1487066340,
      "category_type": "shop"
    },
    {
      "id": 2,
      "name": "Рынок Украины",
      "sort": 2,
      "created_at": 1487066350,
      "updated_at": 1487066350,
      "category_type": null
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.loc/api/v1/content/category/list-main?page=1&per-page=10"
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