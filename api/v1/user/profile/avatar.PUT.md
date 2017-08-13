Обновить аватар пользователя
=============================

`PUT /api/v1/user/profile/avatar`

## Принимаемые заголовки

| Название                   | Значение                        | Обязательность                       |
|----------------------------|---------------------------------|--------------------------------------|
| Content-Type               | application/json                | +                                    |
| Authorization              | Bearer auth_token               | +                                    |


## Принимаемые поля

| Поле                       | Тип                             | Описание                             | Обязательность |
|----------------------------|---------------------------------|--------------------------------------|----------------|
| base64_image               | string(base64)                  | Автарка пользователя                 | +              |

Пример ответа `PUT /api/v1/user/profile/avatar`
----------------------------------------

```json
{
    "status": 200,
    "message": "Аватар успешно изменён",
    "data": {
        "profile": {
            "nickname": "Batman",
            "avatar": "https://s3.eu-central-1.amazonaws.com/assets-dev.ourcnc.com/user_profile/user-10/lcxZIl4wlqQw-7f-pTvVPpoqPCSSDQ14.jpeg",
            "communication_status": "Болтун",
            "date_of_registration": "1490927040",
            "gender": "Мужской",
            "date_of_birth": {
                "day": 15,
                "month": 5,
                "year": 1993
            },
            "reputation": 135,
            "status_message": "Life is good!"
        },
        "statistics": {
            "count_of_likes": 0,
            "count_of_comments": 1,
            "count_of_reviews": 3
        }
    }
}
```