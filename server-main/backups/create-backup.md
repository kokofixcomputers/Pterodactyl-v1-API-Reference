# Create Backup

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/backups`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/backups`

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
  "object": "backup",
  "attributes": {
    "uuid": "63087048-eada-419c-ad72-803c1c949cac",
    "name": "Backup at 2020-07-19 16:21:34",
    "ignored_files": [],
    "sha256_hash": null,
    "bytes": 0,
    "created_at": "2020-07-19T16:21:34+01:00",
    "completed_at": null
  }
}
```
{% endtab %}
{% endtabs %}
