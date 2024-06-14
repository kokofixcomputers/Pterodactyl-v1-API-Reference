# List Backup

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/backups`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/backups`

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
  "object": "list",
  "data": [
    {
      "object": "backup",
      "attributes": {
        "uuid": "904df120-a66f-4375-a4ae-40eedbeae630",
        "name": "Quick Backup",
        "ignored_files": [],
        "sha256_hash": "7c20d6a269b441a9dfd044e3f8ad13d77c09c83af8832d29ad603084a9a63726",
        "bytes": 114402862,
        "created_at": "2020-06-13T05:21:01+01:00",
        "completed_at": "2020-06-13T05:21:04+01:00"
      }
    },
    {
      "object": "backup",
      "attributes": {
        "uuid": "63087048-eada-419c-ad72-803c1c949cac",
        "name": "Backup at 2020-07-19 16:21:34",
        "ignored_files": [],
        "sha256_hash": "39bf93b9d8aee45316fa7ec8bbed0530904558851fa8e712452845c969873b16",
        "bytes": 114567250,
        "created_at": "2020-07-19T16:21:34+01:00",
        "completed_at": "2020-07-19T16:21:35+01:00"
      }
    }
  ],
  "meta": {
    "pagination": {
      "total": 2,
      "count": 2,
      "per_page": 20,
      "current_page": 1,
      "total_pages": 1,
      "links": {}
    }
  }
}
```
{% endtab %}
{% endtabs %}
