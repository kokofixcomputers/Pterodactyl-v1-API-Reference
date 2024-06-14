---
description: Get Generates websocket credentials
---

# Generates websocket credentials

**Request method: GET**

Request Example: \`https://pterodactyl/api/client/servers/\<Server ID>/websocket\`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/websocket`

After you've done this, you can go check out [websocket.md](../websocket.md "mention") for instructions on how to connect.

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
  "data": {
    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6Ij...",
    "socket": "wss:\/\/pterodactyl\/api\/servers\/1a7ce997-259b-452e-8b4e-cecc464142ca\/ws"
  }
}
```
{% endtab %}
{% endtabs %}
