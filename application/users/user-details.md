# User details

<mark style="color:green;">`GET`</mark> `/api/application/users/<userid>`

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
}
```
{% endtab %}
{% endtabs %}
