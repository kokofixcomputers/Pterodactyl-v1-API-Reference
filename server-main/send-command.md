---
description: Send an command to terminal
---

# Send Command

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/command`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/command`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body:**

```json
{
  "command": "<Command (eg: say hi)>"
}
```

**Response should be 204 (No Content) if successes**
