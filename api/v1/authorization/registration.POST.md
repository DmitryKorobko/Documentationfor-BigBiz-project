Регистрация пользователя и магазина
========================

`POST /api/v1/authorization/register`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| email              | string               | Email                                         | +              |
| password_hash      | string               | Пароль                                        | +              |
| confirm            | string               | Пароль еще раз                                | +              |
| role               | ENUM('user', 'shop') | Роль пользователя                             | +              |
| terms_confirm      | boolean              | Принятие соглашения                           | +              |
| name               | string               | Name                                          | +              |


Пример ответа `POST /api/v1/authorization/register`
-----------------------------------------

```json
{
    "status": 201,
    "message": "Регистрация пользователя прошла успешно",
    "data": {
        "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6MjgsImV4cCI6MTQ4NTI3MTU5Mn0.8XtvUrdM5lsCLooxbyck_AKI7teDiWBoSOGe-FLd9Dw",
        "refresh_token": "NmU4OTAwY2RlYTdkZGEwOWRiZTRjM2RhNTg5MWEzMzhhZWJmNzc4MmEzZDQ0NWY0M2NmMzBlZTJjMGQ4NGRlZQ==",
        "user": {
            "id": 28,
            "email": "user2221@gmail.com",
            "status": "VERIFIED || UNVERIFIED",
            "role": "user",
            "name": "DNS",
            "created_at": 1484666791,
            "updated_at": 1484666791
        }
    }
}
```

