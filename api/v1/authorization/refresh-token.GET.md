Авторизация пользователя
========================

`GET /api/v1/authorization/refresh`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа
-------------

```json
{
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6MTQsImV4cCI6MTQ4MjI0MzIyM30.iSATPh-s3zHyj_yA-jEzzQrMyk3aGIQzsc8S5tcSXyE",
    "exp": 1482243113,
    "user": {
        "id": 14,
        "email": "demonic91@mail.ru",
        "role": null,
        "created_at": 1479668046
    }
}
```