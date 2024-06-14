# Create schedule

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/schedules`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/schedules`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Request Body**

```json
{
  "name": "Minute Hello",
  "minute": "*",
  "hour": "*",
  "day_of_month": "*",
  "day_of_week": "*",
  "is_active": true
}
```

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "server_schedule",
  "attributes": {
    "id": 4,
    "name": "Minute Hello",
    "cron": {
      "day_of_week": "*",
      "day_of_month": "*",
      "hour": "*",
      "minute": "*"
    },
    "is_active": true,
    "is_processing": false,
    "last_run_at": null,
    "next_run_at": "2020-06-13T15:17:00+01:00",
    "created_at": "2020-06-13T15:16:45+01:00",
    "updated_at": "2020-06-13T15:16:45+01:00",
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
