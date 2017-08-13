Генерация нового access-token на основе refresh-token
==================================

`POST /api/v1/authorization/generation-access-token`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                                      | Обязательность |
|--------------------|----------------------|-----------------------------------------------|----------------|
| refresh_token      | string               | Refresh token                                 | +              |

## Пример ответа `POST /api/v1/authorization/generation-access-token`

```json
{
    "status": 201,
    "message": "Токен успешно сгенерирован",
    "data": {
        "access_token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6MywiZXhwIjoxNTAwODgwOTc4fQ.LdAoz2bfsInXAs1MrUKn6EIbqM9gLQJ22BjcCh4x7Wo",
        "refresh_token": "NjJiNjc2NTBmMTJlNzZhY2I3MzljYWMxNDRlODllZWMyYjE2YTQ0YmI2NTc1MWJiMGViZTVkOGI0MjY0NGJjNA==",
        "exp": 1500880978,
        "user": {
            "id": 3,
            "email": "timur@mail.ru",
            "role": null,
            "status": "VERIFIED",
            "created_at": 1495533685
        }
    }
}
```
