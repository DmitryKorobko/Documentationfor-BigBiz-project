Like или Dislike темы
========================

`POST /api/v1/theme/like-dislike`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |

## Принимаемые поля

| Поле               | Тип                  | Описание                 | Обязательность |
|--------------------|----------------------|--------------------------|----------------|
| theme_id           | integer              | Theme ID                 | +              |
| like               | integer              | like or dislike (0 || 1) | +              |

## Пример ответа `POST /api/v1/theme/like-dislike`

```json
{
    "status": 200,
    "message": "Like упешно добавлен"
}
```