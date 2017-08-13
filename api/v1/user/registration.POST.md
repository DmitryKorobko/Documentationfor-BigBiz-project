Регистрация пользователя
========================

`POST /api/v1/user/register`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| email              | string               | Email                                         | +              |
| nickname           | string               | Никнейм                                       | +              |
| password_hash      | string               | Пароль                                        | +              |
| confirm            | string               | Пароль еще раз                                | +              |
| role               | ENUM('user')         | Роль пользователя                             | +              |
| terms_confirm      | boolean              | Принятие соглашения                           | +              |


Пример ответа `POST /api/v1/user/register`
-----------------------------------------

```json
{
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6MjgsImV4cCI6MTQ4NTI3MTU5Mn0.8XtvUrdM5lsCLooxbyck_AKI7teDiWBoSOGe-FLd9Dw",
    "user": {
        "id": 28,
        "email": "user2221@gmail.com",
        "status": "VERIFIED || UNVERIFIED",
        "role": "user",
        "created_at": 1484666791,
        "updated_at": 1484666791
    }
}
```

