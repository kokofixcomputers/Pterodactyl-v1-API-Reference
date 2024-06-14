# Create database

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/databases`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/databases`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body:**

```json
{
  "database": "<Database Name>",
  "remote": "<Allowed IPs to access database, use % for all>"
}
```

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
    "name": "bans",
    "username": "u5_aeZqbGdCM9",
    "connections_from": "%",
    "max_connections": 0,
    "relationships": {
      "password": {
        "object": "database_password",
        "attributes": {
          "password": "=lR2orDOcwfKkM=BXb.BVF.C"
        }
      }
    }
  }
}
```
{% endtab %}
{% endtabs %}
