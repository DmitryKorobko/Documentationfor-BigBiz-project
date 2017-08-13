Детальная информация темы
===================

`GET /api/v1/theme/detail?id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/theme/detail?id=10`
--------------------------------------------------

```json
{
  "id": 10,
  "category_name": "Похудение",
  "name": "Скакалка",
  "description": "Прыжки на скакалке для похудения",
  "image": "/admin/images/uploads/user-8/theme/PT22xgaSBWFpIbXgNVqTuNnXhlxXfc1Y.jpg",
  "view_count": 0,
  "comments_count": 0,
  "date_of_publication": 1496918269,
  "is_favorite": false,
  "count_like": 2,
  "count_dislike": 0,
  "is_like": true,
  "is_dislike": false,
  "user_name": "Velo Mag"
}
```