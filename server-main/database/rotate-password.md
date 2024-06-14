---
description: Generate a new password for a database
---

# Rotate Password

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/databases/<Database id>/rotate-password`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/databases/<database id>/rotate-password`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "server_database",
  "attributes": {
    "id": "y9YVxO4V",
    "host": {
      "address": "127.0.0.1",
      "port": 3306
    },
    "name": "s5_punishments",
    "username": "u5_aeZqbGdCM9",
    "connections_from": "%",
    "max_connections": 0,
    "relationships": {
      "password": {
        "object": "database_password",
        "attributes": {
          "password": "vnFKXlJ.p77!EiGR+Kd3muB."
        }
      }
    }
  }
}
```
{% endtab %}
{% endtabs %}
