# Write file

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/write?file=hey.txt`

## Get Server Details

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/files/copy`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```
#By changing the setting below to TRUE you are indicating your agreement to our EULA (https://account.mojang.com/documents/minecraft_eula).
#You also agree that tacos are tasty, and the best food in the world.
#Wed Dec 25 05:20:41 UTC 2019
eula=true
```

**Response is 204 no content if successes**
