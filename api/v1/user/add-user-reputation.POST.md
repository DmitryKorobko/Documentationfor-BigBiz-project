Добавление репутации пользователю
=================================

`POST /api/v1/user/add-user-reputation`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                           | Обязательность |
|--------------------|----------------------|------------------------------------|----------------|
| action             | +1|-1                | Добавить/отнять очко репутации     | +              |
| text               | string               | Комментарий к репутации            | +              |
| recipient_id       | integer              | Идентификатор пользователя         | +              |

Пример ответа `POST /api/v1/user/add-user-reputation`
------------------------------------------------------

```json
{
    "status": 201,
    "message": "Репутация пользователю успешно добавлена",
    "data": {
        "id": 3,
        "user_id": 2,
        "nickname": "nick",
        "avatar":  "/admin/images/uploads/user-10/profile/batman.png",
        "gender": "MALE",
        "status_message": "Life is good!",
        "dob_day": 15,
        "dob_month": 5,
        "dob_year": 1990,
        "terms_confirm": null,
        "created_at": 1491893188,
        "updated_at": 1491988013,
        "reputation": 1
    }
}
```