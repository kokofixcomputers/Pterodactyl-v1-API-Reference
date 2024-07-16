# Node Details

<mark style="color:green;">`GET`</mark> `/api/application/nodes/1`

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
  "object": "node",
  "attributes": {
    "id": 1,
    "uuid": "1046d1d1-b8ef-4771-82b1-2b5946d33397",
    "public": true,
    "name": "Test",
    "description": "Test",
    "location_id": 1,
    "fqdn": "pterodactyl.file.properties",
    "scheme": "https",
    "behind_proxy": false,
    "maintenance_mode": false,
    "memory": 2048,
    "memory_overallocate": 0,
    "disk": 5000,
    "disk_overallocate": 0,
    "upload_size": 100,
    "daemon_listen": 8080,
    "daemon_sftp": 2022,
    "daemon_base": "\/srv\/daemon-data",
    "created_at": "2019-12-22T04:44:51+00:00",
    "updated_at": "2019-12-22T04:44:51+00:00"
  }
}
```
{% endtab %}
{% endtabs %}
