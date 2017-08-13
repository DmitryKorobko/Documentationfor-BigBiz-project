Удаление темы
==============

`DELETE /api/v1/user/theme/{id}`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Пример ответа `DELETE /api/v1/user/theme/6`

``` json
{
    "status": 200,
    "message": "Тема успешно удалена",
    "data": {
        "theme_id": 6
    }
}
```