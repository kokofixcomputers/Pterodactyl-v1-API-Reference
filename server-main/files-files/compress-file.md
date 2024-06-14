# Compress File

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/compress`

## Get Server Details

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/files/compress`

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
  "files": [
    "abc"
  ]
}
```

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "file_object",
  "attributes": {
    "name": "archive-2020-08-23T220805Z.tar.gz",
    "mode": "-rw-------",
    "size": 0,
    "is_file": true,
    "is_symlink": false,
    "is_editable": false,
    "mimetype": "application\/tar+gzip",
    "created_at": "2020-08-23T22:08:05+00:00",
    "modified_at": "2020-08-23T22:08:05+00:00"
  }
}
```
{% endtab %}
{% endtabs %}
