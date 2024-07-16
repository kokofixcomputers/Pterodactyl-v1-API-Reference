# List Users

<mark style="color:green;">`GET`</mark> `/api/application/users`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "list",
  "data": [
    {
      "object": "user",
      "attributes": {
        "id": 1,
        "external_id": "RemoteId1",
        "uuid": "4de5a357-ed95-426b-aec1-8c328cfe9751",
        "username": "admin",
        "email": "example@example.com",
        "first_name": "Admin",
        "last_name": "User",
        "language": "en",
        "root_admin": true,
        "2fa": false,
        "created_at": "2019-12-22T04:43:29+00:00",
        "updated_at": "2020-07-13T13:10:23+00:00"
      }
    },
    {
      "object": "user",
      "attributes": {
        "id": 2,
        "external_id": null,
        "uuid": "73f233ca-99e0-47a9-bd46-efd3296d7ad9",
        "username": "subuser1uxk",
        "email": "subuser1@example.com",
        "first_name": "Server",
        "last_name": "Subuser",
        "language": "en",
        "root_admin": false,
        "2fa": false,
        "created_at": "2020-06-12T22:18:43+00:00",
        "updated_at": "2020-06-12T22:18:43+00:00"
      }
    },
    {
      "object": "user",
      "attributes": {
        "id": 3,
        "external_id": null,
        "uuid": "60a7aec3-e17d-4aa9-abb3-56d944d204b4",
        "username": "subuser2jvc",
        "email": "subuser2@example.com",
        "first_name": "Server",
        "last_name": "Subuser",
        "language": "en",
        "root_admin": false,
        "2fa": false,
        "created_at": "2020-06-12T22:31:41+00:00",
        "updated_at": "2020-06-12T22:31:41+00:00"
      }
    },
    {
      "object": "user",
      "attributes": {
        "id": 4,
        "external_id": null,
        "uuid": "a14e9c5f-9c7a-448f-9106-58e2b5286de6",
        "username": "test",
        "email": "example2@example.com",
        "first_name": "Test",
        "last_name": "Admin",
        "language": "en",
        "root_admin": true,
        "2fa": false,
        "created_at": "2020-06-14T00:34:50+00:00",
        "updated_at": "2020-06-14T00:34:50+00:00"
      }
    },
    {
      "object": "user",
      "attributes": {
        "id": 5,
        "external_id": null,
        "uuid": "1287632d-9224-40c0-906e-f543423400bc",
        "username": "subuser3bvo",
        "email": "subuser3@example.com",
        "first_name": "Server",
        "last_name": "Subuser",
        "language": "en",
        "root_admin": false,
        "2fa": false,
        "created_at": "2020-07-13T13:27:46+00:00",
        "updated_at": "2020-07-13T13:27:46+00:00"
      }
    },
    {
      "object": "user",
      "attributes": {
        "id": 6,
        "external_id": null,
        "uuid": "2fcb6f7e-342a-423a-93a4-6111a237c0c7",
        "username": "geboc70057d6r",
        "email": "geboc70057@djemail.net",
        "first_name": "Server",
        "last_name": "Subuser",
        "language": "en",
        "root_admin": false,
        "2fa": false,
        "created_at": "2020-07-13T13:36:44+00:00",
        "updated_at": "2020-07-13T13:36:44+00:00"
      }
    },
    {
      "object": "user",
      "attributes": {
        "id": 7,
        "external_id": null,
        "uuid": "b20e4e11-550f-4c52-893d-94fc8bc46a06",
        "username": "testidq",
        "email": "test@example.com",
        "first_name": "Server",
        "last_name": "Subuser",
        "language": "en",
        "root_admin": false,
        "2fa": false,
        "created_at": "2020-07-19T12:48:38+00:00",
        "updated_at": "2020-07-19T12:48:38+00:00"
      }
    }
  ],
  "meta": {
    "pagination": {
      "total": 7,
      "count": 7,
      "per_page": 50,
      "current_page": 1,
      "total_pages": 1,
      "links": {}
    }
  }
}
```
{% endtab %}
{% endtabs %}
