---
description: Request an power action
---

# Request a power action

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/power`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/power`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body:**

```json
{
  "signal": "<kill/start/stop/restart>"
}
```

**Response should be 204 (No Content) if successes**
