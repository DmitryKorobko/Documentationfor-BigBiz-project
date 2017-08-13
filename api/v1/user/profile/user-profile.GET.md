Подробная информация о профиле
==============================

`GET /api/v1/user/profile/user-profile?user_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/user/profile/user-profile?user_id=9`
-----------------------------------------------------------

```json
{
  "profile": {
    "nickname": "bbuserbb",
    "avatar": "/admin/images/uploads/user-9/profile/witcher.png",
    "date_of_registration": "1490926925",
    "gender": "Мужской",
    "date_of_birth": {
      "day": "12",
      "month": "6",
      "year": "1987"
    },
    "reputation": "1",
    "status_message": "I'm super user, because I'm BBUSERBB!",
    "communication_status": "Молчун"
  },
  "statistics": {
    "count_of_likes": 5,
    "count_of_comments": "0",
    "count_of_reviews": 3
  }
}
```
