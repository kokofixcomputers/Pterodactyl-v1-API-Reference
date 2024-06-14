---
description: Get Resource usage
---

# Resource usage

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/resources`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/resources`

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
  "object": "stats",
  "attributes": {
    "current_state": "starting",
    "is_suspended": false,
    "resources": {
      "memory_bytes": 588701696,
      "cpu_absolute": 0,
      "disk_bytes": 130156361,
      "network_rx_bytes": 694220,
      "network_tx_bytes": 337090
    }
  }
}
```
{% endtab %}
{% endtabs %}
