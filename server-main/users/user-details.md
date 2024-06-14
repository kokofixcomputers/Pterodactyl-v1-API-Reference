# User details

**Request method: GET**

Request Example:`https://pterodactyl/api/client/servers/<server id>/users/<user id>`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<server id>/users/<user id>`

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
  "object": "server_subuser",
  "attributes": {
    "uuid": "60a7aec3-e17d-4aa9-abb3-56d944d204b4",
    "username": "subuser2jvc",
    "email": "subuser2@example.com",
    "image": "https:\/\/gravatar.com\/avatar\/3bb1c751a8b3488f4a4c70eddfe898d8",
    "2fa_enabled": false,
    "created_at": "2020-06-12T23:31:41+01:00",
    "permissions": [
      "control.console",
      "control.start",
      "websocket.connect"
    ]
  }
}
```
{% endtab %}
{% endtabs %}
