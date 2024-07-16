# Add node

<mark style="color:yellow;">`POST`</mark> `/api/application/nodes`

**Request Body**

```json
{
  "name": "New Node",
  "location_id": 1,
  "fqdn": "node2.example.com",
  "scheme": "https",
  "memory": 10240,
  "memory_overallocate": 0,
  "disk": 50000,
  "disk_overallocate": 0,
  "upload_size": 100,
  "daemon_sftp": 2022,
  "daemon_listen": 8080
}
```

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Response**

{% tabs %}
{% tab title="201" %}
```json

{
  "object": "node",
  "attributes": {
    "id": 4,
    "uuid": "4158cfe9-2aa8-4812-bf6e-d88beeb08e98",
    "public": true,
    "name": "New Node",
    "description": null,
    "location_id": 1,
    "fqdn": "node2.example.com",
    "scheme": "https",
    "behind_proxy": false,
    "maintenance_mode": false,
    "memory": 10240,
    "memory_overallocate": 0,
    "disk": 50000,
    "disk_overallocate": 0,
    "upload_size": 100,
    "daemon_listen": 8080,
    "daemon_sftp": 2022,
    "daemon_base": "\/var\/lib\/pterodactyl\/volumes",
    "created_at": "2020-10-29T01:17:38+00:00",
    "updated_at": "2020-10-29T01:17:38+00:00",
    "allocated_resources": {
      "memory": 0,
      "disk": 0
    }
  },
  "meta": {
    "resource": "https:\/\/pterodactyl.file.properties\/api\/application\/nodes\/4"
  }
}
```
{% endtab %}
{% endtabs %}
