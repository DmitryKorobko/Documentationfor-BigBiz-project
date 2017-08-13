Список мазазинов
==============================

`GET /api/v1/shop/list`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


## Возможные фильтры

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| name               | Пример: Velo         | -              |
| city               | Пример: 1            | -              |

Пример ответа `GET /api/v1/shop/list?name=Velo&city=4`
-----------------------------------------------------------

```json
{
  "items": [
    {
      "id": 8,
      "name": "Velo Mag",
      "image": "/admin/images/uploads/user-8/profile/b7chYJ8exD07m3F0jyzj7MpvSP-hZcLu.jpg",
      "status_text": "Our shop - it's the best bikes!",
      "user_id": 8,
      "cities": [
        {
          "id": 3,
          "name": "Киев"
        },
        {
          "id": 4,
          "name": "Харьков"
        },
        {
          "id": 5,
          "name": "Одесса"
        }
      ],
      "rating": 4.5,
      "is_online": false
    },
    {
      "id": 9,
      "name": "Velo Style",
      "image": "/admin/images/uploads/user-11/profile/I9PY7miPzqrYPJyJoCzgqH8bLk1b5jiM.jpg",
      "status_text": "Our company - is many mountain bikes",
      "user_id": 11,
      "cities": [
        {
          "id": 3,
          "name": "Киев"
        },
        {
          "id": 4,
          "name": "Харьков"
        },
        {
          "id": 5,
          "name": "Одесса"
        },
        {
          "id": 8,
          "name": "Львов"
        }
      ],
      "rating": 0,
      "is_online": false
    }
  ],
  "_links": {
    "self": {
      "href": "http://api/v1/shop/list?name=Velo&city=4&page=1&per-page=10"
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