---
description: assign a new allocation if auto-assign is enabled on the instance
---

# Assign allocations

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/network/allocations`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/schedules/network/allocations`

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
  "object": "allocation",
  "attributes": {
    "id": 6,
    "ip": "45.86.168.218",
    "ip_alias": null,
    "port": 25570,
    "notes": null,
    "is_default": false
  }
}
```
{% endtab %}
{% endtabs %}
