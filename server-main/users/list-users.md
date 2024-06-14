# List Users

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/users`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/users`

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
      "object": "server_subuser",
      "attributes": {
        "uuid": "73f233ca-99e0-47a9-bd46-efd3296d7ad9",
        "username": "subuser1uxk",
        "email": "subuser1@example.com",
        "image": "https:\/\/gravatar.com\/avatar\/c0da5391b64449c1ecbfd4349184377c",
        "2fa_enabled": false,
        "created_at": "2020-06-12T23:18:43+01:00",
        "permissions": [
          "control.console",
          "control.start",
          "control.stop",
          "control.restart",
          "user.create",
          "user.update",
          "user.delete",
          "user.read",
          "file.create",
          "file.read",
          "file.update",
          "file.delete",
          "file.archive",
          "file.sftp",
          "backup.create",
          "backup.read",
          "backup.delete",
          "backup.update",
          "backup.download",
          "allocation.update",
          "startup.update",
          "startup.read",
          "database.create",
          "database.read",
          "database.update",
          "database.delete",
          "database.view_password",
          "schedule.create",
          "schedule.read",
          "schedule.update",
          "settings.rename",
          "schedule.delete",
          "settings.reinstall",
          "websocket.connect"
        ]
      }
    },
    {
      "object": "server_subuser",
      "attributes": {
        "uuid": "60a7aec3-e17d-4aa9-abb3-56d944d204b4",
        "username": "subuser2jvc",
        "email": "subuser2@example.com",
        "image": "https:\/\/gravatar.com\/avatar\/3bb1c751a8b3488f4a4c70eddfe898d8",
        "2fa_enabled": false,
        "created_at": "2020-06-12T23:31:41+01:00",
        "permissions": [
          "control.console",
          "control.start",
          "websocket.connect"
        ]
      }
    },
    {
      "object": "server_subuser",
      "attributes": {
        "uuid": "1287632d-9224-40c0-906e-f543423400bc",
        "username": "subuser3bvo",
        "email": "subuser3@example.com",
        "image": "https:\/\/gravatar.com\/avatar\/8b28d32aaa64a1564450d16f71a81f65",
        "2fa_enabled": false,
        "created_at": "2020-07-13T14:27:46+01:00",
        "permissions": [
          "control.console",
          "control.start",
          "websocket.connect"
        ]
      }
    },
    {
      "object": "server_subuser",
      "attributes": {
        "uuid": "2fcb6f7e-342a-423a-93a4-6111a237c0c7",
        "username": "geboc70057d6r",
        "email": "geboc70057@djemail.net",
        "image": "https:\/\/gravatar.com\/avatar\/354d25d88e2c73b9f8d8e9bb8f1bf15e",
        "2fa_enabled": false,
        "created_at": "2020-07-13T14:36:44+01:00",
        "permissions": [
          "control.console",
          "control.start",
          "websocket.connect"
        ]
      }
    },
    {
      "object": "server_subuser",
      "attributes": {
        "uuid": "b20e4e11-550f-4c52-893d-94fc8bc46a06",
        "username": "testidq",
        "email": "test@example.com",
        "image": "https:\/\/gravatar.com\/avatar\/55502f40dc8b7c769880b10874abc9d0",
        "2fa_enabled": false,
        "created_at": "2020-07-19T13:48:38+01:00",
        "permissions": [
          "control.*",
          "websocket.connect"
        ]
      }
    }
  ]
}
```
{% endtab %}
{% endtabs %}
