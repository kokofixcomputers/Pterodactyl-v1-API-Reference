# Register User

<mark style="color:yellow;">`POST`</mark> `/api/application/users`

**Request Body**

```json
{
  "email": "example10@example.com",
  "username": "exampleuser",
  "first_name": "Example",
  "last_name": "User"
}
```

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
    "external_id": null,
    "uuid": "dac03ece-fd51-4e4b-bd4f-a79e3b2794f9",
    "username": "exampleuser",
    "email": "example10@example.com",
    "first_name": "Example",
    "last_name": "User",
    "language": "en",
    "root_admin": false,
    "2fa": false,
    "created_at": "2020-10-29T01:25:12+00:00",
    "updated_at": "2020-10-29T01:25:12+00:00"
  },
  "meta": {
    "resource": "https:\/\/pterodactyl.file.properties\/api\/application\/users\/9"
  }
}
```
{% endtab %}
{% endtabs %}
