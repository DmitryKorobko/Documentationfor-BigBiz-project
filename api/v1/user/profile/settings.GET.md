Метод получения настроек профиля пользователя
=============================================

`GET /api/v1/user/profile/settings`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/user/profile/settings`
-----------------------------------------------------------

```json
{
  "avatar": "/admin/images/uploads/user-10/profile/batman.png",
  "status_message": "Life is good!",
  "personal_information": {
    "email": "batman@gmail.com",
    "nickname": "Batman",
    "gender": "MALE",
    "date_of_birth": {
      "day": 15,
      "month": 5,
      "year": 1993
    }
  },
  "confidentiality": {
    "show_date_of_birth": 1,
    "show_status_online": 1,
    "view_page_access": "ALL_USERS",
    "send_messages_access": "ALL_USERS",
    "frequency_history_cleaning": "SEVEN_DAYS"
  },
  "notifications_settings": {
    "new_personal_message": 1,
    "new_reputation": 1,
    "new_reply_comment": 1,
    "new_product_report": 1,
    "new_theme_comment": 1,
    "theme_was_verified": 1,
    "new_like": 1,
    "messages_to_email": 1,
    "site_dispatch": 1
  }
}
```