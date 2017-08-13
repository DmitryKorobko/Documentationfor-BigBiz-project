Подробная информация о профиле
==============================

`GET /api/v1/user/profile`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/user/profile`
-----------------------------------------------------------

```json
{
  "profile": {
    "nickname": "Batman",
    "avatar": "/admin/images/uploads/user-10/profile/batman.png",
    "date_of_registration": 1490927040,
    "gender": "Мужской",
    "date_of_birth": {
      "day": 15,
      "month": 5,
      "year": 1993
    },
    "reputation": 2,
    "status_message": "Life is good!",
    "communication_status": "Болтун"
  },
  "statistics": {
    "count_of_likes": 0,
    "count_of_comments": 1,
    "count_of_reviews": 3
  }
}
```
