Метод бокового меню пользователя
================================
   
`GET /api/v1/user/profile/side-menu`
   
## Принимаемые заголовки
   
| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |
   
   
Пример ответа `GET /api/v1/user/profile/side-menu`
--------------------------------------------------
   
```json
{
  "user_id": 10,
  "nickname": "Batman",
  "avatar": "/admin/images/uploads/user-10/profile/batman.png",
  "count_new_messages": 0,
  "count_new_answers": 1
}
```