# Update schedule

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/schedules/<schedule id>`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/schedules/<schedule id>`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```json
{
  "name": "Hourly Hello",
  "minute": "0",
  "hour": "*",
  "day_of_month": "*",
  "day_of_week": "*"
}
```

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "server_schedule",
  "attributes": {
    "id": 2,
    "name": "Hourly Hello",
    "cron": {
      "day_of_week": "*",
      "day_of_month": "*",
      "hour": "*",
      "minute": "0"
    },
    "is_active": false,
    "is_processing": false,
    "last_run_at": null,
    "next_run_at": "2020-06-13T16:00:00+01:00",
    "created_at": "2020-06-13T15:05:25+01:00",
    "updated_at": "2020-06-13T15:14:07+01:00",
    "relationships": {
      "tasks": {
        "object": "list",
        "data": []
      }
    }
  }
}
```
{% endtab %}
{% endtabs %}
