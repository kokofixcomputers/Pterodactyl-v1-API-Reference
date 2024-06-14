# Set/Update Variable

**Request method: PUT**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/startup/variable`

<mark style="color:orange;">`PUT`</mark> `/api/client/servers/<Server ID>/startup/variable`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```json
{
  "key": "SERVER_JARFILE",
  "value": "server.jar"
}
```

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "egg_variable",
  "attributes": {
    "name": "Server Jar File",
    "description": "The name of the server jarfile to run the server with.",
    "env_variable": "SERVER_JARFILE",
    "default_value": "server.jar",
    "server_value": "server.jar",
    "is_editable": true,
    "rules": "required|regex:\/^([\\w\\d._-]+)(\\.jar)$\/"
  }
}
```
{% endtab %}
{% endtabs %}
