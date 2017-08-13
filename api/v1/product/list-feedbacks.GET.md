Список отзывов о товаре
=======================

`GET /api/v1/product/list-reviews?product_id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/product/list-reviews?product_id=1`
-------------

```json
{
  "items": [
    {
        "id": 1,
        "product_id": 1,
        "user_id": 1,
        "text": "The product page is the last item in the sales funnel before the user clicks place order",
        "rating": 1,
        "created_at": 1234123,
        "status_online": 1,
        "nickname": "guest",
        "avatar": "https://s3.eu-central-1.amazonaws.com/assets-dev.ourcnc.com/user_profile/user-10/lcxZIl4wlqQw-7f-pTvVPpoqPCSSDQ14.jpeg",
        "likes_count": 2
    },
    {
        "id": 2,
        "product_id": 1,
        "user_id": 3,
        "text": "The description of the product is the main reason for purchase. On whether you can convince the visitor of the need for your product depends on whether he buys it or not.",
        "rating": 2,
        "created_at": 1234123,
        "status_online": 1,
        "nickname": "bob",
        "avatar": null,
        "likes_count": 2
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.com/api/v1/product/list-feedbacks?product_id=1&page=1&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 7,
    "pageCount": 1,
    "currentPage": 1,
    "perPage": 10
  }
}