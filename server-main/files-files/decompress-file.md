# Decompress File

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/decompress`

## Get Server Details

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/files/decompress`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```json
{
  "root": "/",
  "file": "archive-2020-08-23T220655Z.tar.gz"
}
```

**Response is 204 no content if successes**
