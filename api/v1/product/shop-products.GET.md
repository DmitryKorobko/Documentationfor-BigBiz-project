Список товаров магазина
=======================

`GET /api/v1/product/list?shop_id=..`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/product/list?shop_id=1`
-------------

```json
{
    "items": [
        {
            "id": "9",
            "name": "ыфвфы",
            "image": "/admin/images/upload/product/eSR2BwWbOWzj6FwrT71FsOk9315BcZEJ.jpg",
            "availability": "0",
            "prices": [
                {
                    "id": "14",
                    "product_id": "9",
                    "count": "1",
                    "price": "10"
                }
            ],
            "is_favorite": false,
            "count_report": "2",
            "average_rating": "4.0000"
        },
        {
            "id": "1",
            "name": "Охуенный таз",
            "description": "<p>Охуенный таз</p>\r\n",
            "image": "/admin/images/upload/product/iCO3gT69bBjvnDKUm1X81dCUO_5fm8m7.jpg",
            "availability": "1",
            "prices": [
                {
                    "id": "40",
                    "product_id": "1",
                    "count": "1",
                    "price": "10"
                }
            ],
            "is_favorite": false,
            "count_report": "3",
            "average_rating": "5.0000"
        },
        {
            "id": "2",
            "name": "Веник охуенный",
            "description": "<p>выаываываываыв</p>\r\n",
            "image": "/admin/images/upload/product/-kxduJ4OP04MqSeBXJlpJWWwE41Mph4t.jpg",
            "availability": "1",
            "prices": [
                {
                    "id": "41",
                    "product_id": "2",
                    "count": "1",
                    "price": "11"
                }
            ],
            "is_favorite": false,
            "count_report": "3",
            "average_rating": "4.0000"
        }
    ],
    "_links": {
        "self": {
            "href": "http://bb.loc//api/v1/shop/products?shop_id=23&page=1&per-page=5"
        }
    },
    "_meta": {
        "totalCount": 5,
        "pageCount": 1,
        "currentPage": 1,
        "perPage": 5
    }
}
```