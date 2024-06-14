# Get allocations

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/network/allocations`

## Get Server Details

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/schedules/network/allocations`

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
      "object": "allocation",
      "attributes": {
        "id": 1,
        "ip": "45.86.168.218",
        "ip_alias": null,
        "port": 25565,
        "notes": null,
        "is_default": true
      }
    },
    {
      "object": "allocation",
      "attributes": {
        "id": 2,
        "ip": "45.86.168.218",
        "ip_alias": null,
        "port": 25566,
        "notes": "Votifier",
        "is_default": false
      }
    }
  ]
}
```
{% endtab %}
{% endtabs %}
