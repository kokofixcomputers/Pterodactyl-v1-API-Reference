# Delete file

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/delete`

## Get Server Details

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/files/delete`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```json
{
  "root": "/maps",
  "files": [
    "worlds"
  ]
}
```

**Response is 204 no content if successes**
