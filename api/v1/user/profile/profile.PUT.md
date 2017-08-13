Обновить профиль пользователя
=============================

`PUT /api/v1/user/profile`

## Принимаемые заголовки

| Название                   | Значение                        | Обязательность                       |
|----------------------------|---------------------------------|--------------------------------------|
| Content-Type               | application/json                | +                                    |
| Authorization              | Bearer auth_token               | +                                    |


## Принимаемые поля

| Поле                       | Тип                             | Описание                             | Обязательность |
|----------------------------|---------------------------------|--------------------------------------|----------------|
| nickname                   | string                          | Nickname                             | -              |
| avatar                     | string(base64)                  | Автарка пользователя                 | -              |
| status_message             | string(50)                      | Текст для статуса                    | -              |
| gender                     | ENUM('MALE', 'FEMALE')          | Пол пользователя (Male, Female)      | -              |
| dob_day                    | integer                         | День рождения                        | -              |
| dob_month                  | integer                         | Месяц рождения                       | -              |
| dob_year                   | integer                         | Год рождения                         | -              |
| show_date_of_birth         | boolean                         | Отображение даты рождения            | -              |
| show_status_online         | boolean                         | Отображение статуса online           | -              |
| view_page_access           | ENUM('ALL_USERS', 'NOBODY',     | Доступ к просмотру страницы          | -              |
|                            |     'REGISTERED_USERS')         |                                      |                |
| send_messages_access       | ENUM('ALL_USERS', 'NOBODY',     | Доступ к отправке личных сообщений   | -              |
|                            |     'REGISTERED_USERS')         |                                      |                |
| frequency_history_cleaning | ENUM('ONE_MINUTE',              | Частота очистки истории сообщений    | -              |
|                            |    'FIVE_MINUTES', 'ONE_HOUR',  |                                      |                |
|                            |    'THREE_HOURS', 'FIVE_HOURS', |                                      |                |
|                            |    'TWELVE_HOURS', 'ONE_DAY',   |                                      |                |
|                            |    'SEVEN_DAYS')                |                                      |                |
| new_personal_message       | boolean                         | Личное сообщение                     | -              |
| new_reputation             | boolean                         | Добавление репутации                 | -              |
| new_reply_comment          | boolean                         | Ответ на комментарий                 | -              |
| new_product_report         | boolean                         | Отзыв об отслеживаемом продукте      | -              |
| new_theme_comment          | boolean                         | Комментарий к отслеживаемой теме     | -              |
| theme_was_verified         | boolean                         | Тема проверена                       | -              |
| new_like                   | boolean                         | Мне нравится                         | -              |
| messages_to_email          | boolean                         | Письмо на email о новых сообщениях   | -              |
| site_dispatch              | boolean                         | Получать рассылку сайта              | -              |

Пример ответа `PUT /api/v1/user/profile`
----------------------------------------

```json
{
    "status": 200,
    "message": "Профиль успешно изменён",
    "data": {
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
            "show_date_of_birth": 0,
            "show_status_online": 0,
            "view_page_access": "ALL_USERS",
            "send_messages_access": "NOBODY",
            "frequency_history_cleaning": "SEVEN_DAYS"
        },
        "notifications_settings": {
            "new_personal_message": 1,
            "new_reputation": 1,
            "new_reply_comment": 1,
            "new_product_report": 1,
            "new_theme_comment": 1,
            "theme_was_verified": 1,
            "new_like": "1",
            "messages_to_email": 0,
            "site_dispatch": 0
        }
    }
}
```