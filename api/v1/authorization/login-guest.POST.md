Авторизация пользователя как гость
==================================

`POST /api/v1/authorization/login-guest`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |


Пример ответа
-------------

```json
{
    "status": 200,
    "message": "Авторизация пользователя как 'гость' прошла успешно",
    "data": {
        "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6MTQsImV4cCI6MTQ4MjI0MzExM30.H_wVbIpFcPS_WAoYgQL8U_InC5-EwKZWZmErUhiZYJM",
        "exp": 1482243113,
        "user": {
            "id": 1,
            "email": "guest@gmail.com",
            "role": "guest",
            "status": "UNVERIFIED",
            "created_at": 1479668046
        }
     }
}
```