Краткая информация о магазине с темами и товарами
=======

`GET /api/v1/shop/preview?shop_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/shop/preview?shop_id=8`
--------------------------------------------------

```json
{
  "id": 8,
  "name": "Velo Mag",
  "image": "/admin/images/uploads/user-8/profile/_-zzqEpE3MiM2PD-UKf5DE3P3f_HBenE.jpg",
  "user_id": 8,
  "user_registration_date": 1490940211,
  "rating": 4.8,
  "is_online": true,
  "themes": [
    {
      "id": 4,
      "category_name": "Экстрим",
      "name": "Даунхилл",
      "shop_name": "Velo Mag",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1492691714,
      "count_like": 1,
      "count_dislike": 0,
      "is_favorite": false,
      "is_like": 0,
      "is_dislike": 0
    },
    {
      "id": 10,
      "category_name": "Похудение",
      "name": "Скакалка",
      "shop_name": "Velo Mag",
      "view_count": 0,
      "comments_count": 0,
      "date_of_publication": 1496918269,
      "count_like": 2,
      "count_dislike": 0,
      "is_favorite": false,
      "is_like": 1,
      "is_dislike": 0
    },
    {
      "id": 2,
      "category_name": "Похудение",
      "name": "Велопрогулка",
      "shop_name": "Velo Mag",
      "view_count": 2,
      "comments_count": 0,
      "date_of_publication": 1492691715,
      "count_like": 2,
      "count_dislike": 0,
      "is_favorite": false,
      "is_like": 0,
      "is_dislike": 0
    }
  ],
  "count_themes": 3,
  "products": [
    {
      "id": 1,
      "name": "Колесо переднее",
      "description": "Колесо переднее для хардтейла стальное в сборе со стальными спицами, стальной втулкой и шиной 26 х 2,25.",
      "image": "/admin/images/uploads/user-8/product/PfiAcWTIII-l5J7pP7yHNAOMe1rmm3-O.jpg",
      "availability": 1,
      "is_favorite": true,
      "count_report": 1,
      "average_rating": "5.0000",
      "price": 1500
    },
    {
      "id": 2,
      "name": "Седло кросс-кантрийное",
      "description": "Кросс-кантрийное седло. Узкое, с небольшой рамкой крепления к подседельному штырю, с жесткостью, от небольшой до &ldquo;дубовой&rdquo;.",
      "image": "/admin/images/uploads/user-8/product/QvjSBMBSt1R3ql7r0F6ZLZ5vnF8I7iaZ.jpg",
      "availability": 0,
      "is_favorite": false,
      "count_report": 2,
      "average_rating": "4.0000",
      "price": 850
    }
  ],
  "count_products": 2
}
```