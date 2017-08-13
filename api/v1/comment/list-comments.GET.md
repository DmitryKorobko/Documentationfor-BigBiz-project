Список комментариев
==============================

`GET /api/v1/comment?theme_id=...`

## Принимаемые заголовки

| Название           | Значение             | Обязательность |
|--------------------|----------------------|----------------|
| Content-Type       | application/json     | +              |
| Authorization      | Bearer auth_token    | +              |


Пример ответа `GET /api/v1/comment?theme_id=1`
-------------------------------------------------------

```json
{
  "items": [
    {
      "recipient": [],
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "15",
        "text": "Hello world",
        "recipient_id": null,
        "created_by": "6",
        "created_at": "1488879943",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "14",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879901",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "13",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879890",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "12",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879877",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "11",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879845",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "10",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879835",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "9",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879806",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "8",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879608",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "7",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879562",
        "status": "UNREAD",
        "count_like": "0"
      }
    },
    {
      "recipient": {
        "name": "My shop"
      },
      "author": {
        "name": "demo",
        "avatar": null
      },
      "comment": {
        "id": "6",
        "text": "Hello world",
        "recipient_id": "4",
        "created_by": "6",
        "created_at": "1488879517",
        "status": "UNREAD",
        "count_like": "0"
      }
    }
  ],
  "_links": {
    "self": {
      "href": "http://bb.loc/api/v1/comment?theme_id=1&page=1&per-page=10"
    },
    "next": {
      "href": "http://bb.loc/api/v1/comment?theme_id=1&page=2&per-page=10"
    },
    "last": {
      "href": "http://bb.loc/api/v1/comment?theme_id=1&page=2&per-page=10"
    }
  },
  "_meta": {
    "totalCount": 14,
    "pageCount": 2,
    "currentPage": 1,
    "perPage": 10
  }
}
```