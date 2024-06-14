# List all databases

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/databases`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/databases`

**Parameters**

| Name       | Description            |
| ---------- | ---------------------- |
| `password` | Database user password |

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
      "object": "server_database",
      "attributes": {
        "id": "bEY4yAD5",
        "host": {
          "address": "127.0.0.1",
          "port": 3306
        },
        "name": "s5_perms",
        "username": "u5_QsIAp1jhvS",
        "connections_from": "%",
        "max_connections": 0
      }
    },
    {
      "object": "server_database",
      "attributes": {
        "id": "E0A0Rw42",
        "host": {
          "address": "127.0.0.1",
          "port": 3306
        },
        "name": "s5_coreprotect",
        "username": "u5_2jtJx1nO1d",
        "connections_from": "%",
        "max_connections": 0
      }
    }
  ]
}
```
{% endtab %}
{% endtabs %}
