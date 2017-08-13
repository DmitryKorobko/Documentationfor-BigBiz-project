Список тем категорий второго уровня
===================

`GET /api/v1/theme/list?category_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/theme/list?category_id=1`
--------------------------------------------------

```json
{
  "items": [
    {
      "id": 1,
      "name": "Пробежка",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-7/theme/9TrHiolQLHhbdLnoGkfCZEMGo3rkbFd4.jpg",
      "view_count": 3,
      "comments_count": 0,
      "date_of_publication": 1492691714,
      "count_like": 1,
      "count_dislike": 2,
      "is_like": 0,
      "is_dislike": 0,
      "user_name": "Rammstein Shop"
    },
    {
      "id": 3,
      "name": "Правильное питание",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-9/theme/r0LFc6icHW97MbW-wXSnm0-RIqkS1FAr.jpg",
      "view_count": 2,
      "comments_count": 0,
      "date_of_publication": 1490956387,
      "count_like": 1,
      "count_dislike": 1,
      "is_like": 0,
      "is_dislike": 0,
      "user_name": "Witcher"
    },
    {
      "id": 6,
      "name": "Зарядка",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-9/theme/HjzuVhCqxqMonwYuMoZg6I7zgtT4ib85.jpg",
      "view_count": 0,
      "comments_count": 1,
      "date_of_publication": 1490941202,
      "count_like": 0,
      "count_dislike": 0,
      "is_like": 0,
      "is_dislike": 0,
      "user_name": "Witcher"
    },
    {
      "id": 7,
      "name": "Плавание",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-10/theme/r0LFc6icHW97MbW-wXSnm0-RIqkS1FAr.jpg",
      "view_count": 0,
      "comments_count": 2,
      "date_of_publication": 1492691715,
      "count_like": 2,
      "count_dislike": 1,
      "is_like": 0,
      "is_dislike": 1,
      "user_name": "Batman"
    },
    {
      "id": 8,
      "name": "Кусочек кода",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-86/theme/IzF17IcSYavJXaZSVZlcb5ZVYjeCUwLG.jpg",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1496847609,
      "count_like": 0,
      "count_dislike": 0,
      "is_like": 0,
      "is_dislike": 0,
      "user_name": "Администрация"
    },
    {
      "id": 10,
      "name": "Скакалка",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-8/theme/PT22xgaSBWFpIbXgNVqTuNnXhlxXfc1Y.jpg",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1496918269,
      "count_like": 2,
      "count_dislike": 0,
      "is_like": 1,
      "is_dislike": 0,
      "user_name": "Velo Mag"
    },
    {
      "id": 2,
      "name": "Велопрогулка",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-8/theme/r0LFc6icHW97MbW-wXSnm0-RIqkS1FAr.jpg",
      "view_count": 2,
      "comments_count": 0,
      "date_of_publication": 1492691715,
      "count_like": 2,
      "count_dislike": 0,
      "is_like": 0,
      "is_dislike": 0,
      "user_name": "Velo Mag"
    },
    {
      "id": 9,
      "name": "Структура проекта",
      "category_name": "Похудение",
      "image": "/admin/images/uploads/user-86/theme/3pOWTaBKKVPWOnoUtIPKAGsVkBIDJ2jv.png",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1496847646,
      "count_like": 0,
      "count_dislike": 0,
      "is_like": 0,
      "is_dislike": 0,
      "user_name": "Администрация"
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/theme/list?category_id=1&page=1&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 8,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 10
  }
}
```