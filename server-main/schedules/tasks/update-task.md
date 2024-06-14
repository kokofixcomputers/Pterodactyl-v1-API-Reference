# Update Task

**Request method: POST**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/schedules/<schedule id>/tasks/<task id>`

<mark style="color:yellow;">`POST`</mark> `/api/client/servers/<Server ID>/schedules/<schedule id>/tasks/<task id>`

**Headers**

| Name            | Value                  |
| --------------- | ---------------------- |
| `Accept`        | application/json       |
| `Content-Type`  | application/json       |
| `Authorization` | Bearer \<Your Api Key> |

**Available Actions**

| Action name | Description           |
| ----------- | --------------------- |
| command     | Run an command        |
| power       | Sends an power action |
| backup      | Create an backup      |

**Request Body**

```json
{
  "action": "command",
  "payload": "say Updated Statement!?",
  "time_offset": "0"
}
```

**Response**

{% tabs %}
{% tab title="200" %}
```json
{
  "object": "schedule_task",
  "attributes": {
    "id": 6,
    "sequence_id": 1,
    "action": "command",
    "payload": "say Hello World",
    "time_offset": 0,
    "is_queued": false,
    "created_at": "2020-10-29T01:09:03+00:00",
    "updated_at": "2020-10-29T01:09:03+00:00"
  }
}
```
{% endtab %}
{% endtabs %}
