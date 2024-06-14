# Schedule details

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/schedules/<schedule id>`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/schedules/<schedule id>`

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
  "object": "server_schedule",
  "attributes": {
    "id": 1,
    "name": "Daily Reboot",
    "cron": {
      "day_of_week": "*",
      "day_of_month": "*",
      "hour": "0",
      "minute": "0"
    },
    "is_active": true,
    "is_processing": false,
    "last_run_at": null,
    "next_run_at": "2020-06-13T00:00:00+01:00",
    "created_at": "2020-06-12T23:50:14+01:00",
    "updated_at": "2020-06-12T23:53:07+01:00",
    "relationships": {
      "tasks": {
        "object": "list",
        "data": [
          {
            "object": "schedule_task",
            "attributes": {
              "id": 1,
              "sequence_id": 1,
              "action": "command",
              "payload": "say Rebooting...",
              "time_offset": 0,
              "is_queued": false,
              "created_at": "2020-06-12T23:50:46+01:00",
              "updated_at": "2020-06-12T23:52:54+01:00"
            }
          },
          {
            "object": "schedule_task",
            "attributes": {
              "id": 2,
              "sequence_id": 2,
              "action": "power",
              "payload": "restart",
              "time_offset": 5,
              "is_queued": false,
              "created_at": "2020-06-12T23:53:07+01:00",
              "updated_at": "2020-06-12T23:53:07+01:00"
            }
          }
        ]
      }
    }
  }
}
```
{% endtab %}
{% endtabs %}
