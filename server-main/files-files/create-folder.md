# Create folder

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/create-folder`

## Get Server Details

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/files/create-folder`

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
  "name": "worlds"
}
```

**Response is 204 no content if successes**
