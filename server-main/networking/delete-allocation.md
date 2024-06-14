# Delete Allocation

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/network/allocations/<allocation id>`

## Get Server Details

<mark style="color:red;">`DELETE`</mark> `/api/client/servers/<Server ID>/schedules/network/allocations/<allocation id>`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Response**

{% tabs %}
{% tab title="204" %}
```json
//Success (no actual response)
```
{% endtab %}

{% tab title="400" %}
```json
{
  "errors": [
    {
      "code": "DisplayException",
      "status": "400",
      "detail": "Cannot delete the primary allocation for a server."
    }
  ]
}
```
{% endtab %}
{% endtabs %}
