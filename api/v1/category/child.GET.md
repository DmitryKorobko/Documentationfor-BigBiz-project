Список категорий второго уровня
================================

`GET /api/v1/category/list-child?parent_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## GET параметры

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| parent_id          | Пример: 1            | +              |
| user_category      | Пример: 1            | -              |

Пример ответа
-------------

```json
{
  "items": [
    {
      "id": 2,
      "name": "Безопасность",
      "sort": 2
    },
    {
      "id": 1,
      "name": "Новости",
      "sort": 5
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.loc/api/v1/category/list-child?parent_id=1&page=1&per-page=10"
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