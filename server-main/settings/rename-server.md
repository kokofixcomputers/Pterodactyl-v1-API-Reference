# Rename Server

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/settings/rename`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/settings/rename`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```json
{
  "name": "Gaming"
}
```

**Response is 204 no content if success**
