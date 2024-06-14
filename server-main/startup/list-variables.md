# List Variables

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/startup`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/startup`

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
  "object": "list",
  "data": [
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
    },
    {
      "object": "egg_variable",
      "attributes": {
        "name": "Server Version",
        "description": "The version of Minecraft Vanilla to install. Use \"latest\" to install the latest version.",
        "env_variable": "VANILLA_VERSION",
        "default_value": "latest",
        "server_value": "latest",
        "is_editable": true,
        "rules": "required|string|between:3,15"
      }
    }
  ],
  "meta": {
    "startup_command": "java -Xms128M -Xmx512M -jar server.jar",
    "raw_startup_command": "java -Xms128M -Xmx\{\{ SERVER_MEMORY }}M -jar {\{ SERVER_JARFILE }}"
  }
}
```
{% endtab %}
{% endtabs %}
