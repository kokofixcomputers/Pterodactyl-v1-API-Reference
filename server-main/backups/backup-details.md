# Backup Details

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/backups/<backup uuid>`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/backups/<backup uuid>`

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
    "uuid": "904df120-a66f-4375-a4ae-40eedbeae630",
    "name": "Quick Backup",
    "ignored_files": [],
    "sha256_hash": "7c20d6a269b441a9dfd044e3f8ad13d77c09c83af8832d29ad603084a9a63726",
    "bytes": 114402862,
    "created_at": "2020-06-13T05:21:01+01:00",
    "completed_at": "2020-06-13T05:21:04+01:00"
  }
}
```
{% endtab %}
{% endtabs %}
