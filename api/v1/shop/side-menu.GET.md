Метод бокового меню магазина
============================
   
`GET /api/v1/shop/side-menu`
   
## Принимаемые заголовки
   
| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |
   
   
Пример ответа `GET /api/v1/shop/side-menu`
--------------------------------------------------
   
```json
{
  "shop_id": 8,
  "name": "Velo Mag",
  "image": "/admin/images/uploads/user-8/profile/b7chYJ8exD07m3F0jyzj7MpvSP-hZcLu.jpg",
  "count_new_messages": 1,
  "count_new_answers": 1,
  "count_new_reviews": 0
}
```