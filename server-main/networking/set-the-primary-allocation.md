# Set the primary allocation

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/network/allocations/<allocation id>/primary`

## Get Server Details

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/schedules/network/allocations/<allocation id>/primary`

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
    "id": 2,
    "ip": "45.86.168.218",
    "ip_alias": null,
    "port": 25566,
    "notes": "Votifier",
    "is_default": true
  }
}
```
{% endtab %}
{% endtabs %}
