# List Nodes

<mark style="color:green;">`GET`</mark> `/api/application/nodes`

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
    },
    {
      "object": "node",
      "attributes": {
        "id": 3,
        "uuid": "71b15cf6-909a-4b60-aa04-abb4c8f98f61",
        "public": true,
        "name": "2",
        "description": "e",
        "location_id": 1,
        "fqdn": "pterodactyl.file.properties",
        "scheme": "https",
        "behind_proxy": false,
        "maintenance_mode": false,
        "memory": 100,
        "memory_overallocate": 0,
        "disk": 100,
        "disk_overallocate": 0,
        "upload_size": 100,
        "daemon_listen": 8080,
        "daemon_sftp": 2022,
        "daemon_base": "\/var\/lib\/pterodactyl\/volumes",
        "created_at": "2020-06-23T04:50:37+00:00",
        "updated_at": "2020-06-23T04:50:37+00:00"
      }
    }
  ],
  "meta": {
    "pagination": {
      "total": 2,
      "count": 2,
      "per_page": 50,
      "current_page": 1,
      "total_pages": 1,
      "links": {}
    }
  }
}
```
{% endtab %}
{% endtabs %}
