Авторизация пользователя
========================

`POST /api/v1/authorization/login`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| email              | string               | Email                                         | +              |
| password_hash      | string               | Пароль                                        | +              |

Пример ответа
-------------

```json
{
    "status": 200,
    "message": "Авторизация прошла успешна",
    "data": {
        "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6MTQsImV4cCI6MTQ4MjI0MzExM30.H_wVbIpFcPS_WAoYgQL8U_InC5-EwKZWZmErUhiZYJM",
        "refresh_token": "MWE0NTRhNzNlZWNhZGNjMjgyZmUyYjk3NGRmNTkzZjMyMTljNTA3YjM4ZGRmYzA3ODk5ZmMxZjAxZmY0MGM0NA==",
        "exp": 1482243113,
        "user": {
            "id": 14,
            "email": "demonic91@mail.ru",
            "role": "user",
            "status": "VERIFIED || UNVERIFIED",
            "created_at": 1479668046
        }
    }
}
```