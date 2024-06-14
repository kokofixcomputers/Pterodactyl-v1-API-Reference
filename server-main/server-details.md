---
description: Get Server Details
---

# Server Details

**Request method: GET**

Request Example: \`https://pterodactyl/api/client/servers/\<Server ID>\`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>`

**Parameters**

| Parameter | Info                                          |
| --------- | --------------------------------------------- |
| egg       | Get information about the egg the server uses |
| subusers  | Lists out the subusers                        |

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
  "object": "server",
  "attributes": {
    "server_owner": true,
    "identifier": "1a911e",
    "uuid": "3a6ce947-259a-452b-8b4e-ceca468142ca",
    "name": "Test Server",
    "node": "Test",
    "sftp_details": {
      "ip": "<Your Ip>",
      "port": 2024
    },
    "description": "Just a test server.",
    "limits": {
      "memory": 1024,
      "swap": 0,
      "disk": 600,
      "io": 700,
      "cpu": 100
    },
    "feature_limits": {
      "databases": 5,
      "allocations": 5,
      "backups": 2
    },
    "is_suspended": false,
    "is_installing": false,
    "relationships": {
      "allocations": {
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
          }
        ]
      }
    }
  },
  "meta": {
    "is_server_owner": true,
    "user_permissions": [
      "*"
    ]
  }
}
```
{% endtab %}
{% endtabs %}
