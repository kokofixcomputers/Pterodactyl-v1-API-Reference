# Get node configuration&#x20;

<mark style="color:green;">`GET`</mark> `/api/application/nodes/1/configuration`

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
  "debug": false,
  "uuid": "1046d1d1-b8ef-4771-82b1-2b5946d33397",
  "token_id": "iAcosCn1KCAgVjVO",
  "token": "FanPzLCptUxkGow3vi7Z",
  "api": {
    "host": "0.0.0.0",
    "port": 8080,
    "ssl": {
      "enabled": true,
      "cert": "\/etc\/letsencrypt\/live\/pterodactyl.file.properties\/fullchain.pem",
      "key": "\/etc\/letsencrypt\/live\/pterodactyl.file.properties\/privkey.pem"
    },
    "upload_limit": 100
  },
  "system": {
    "data": "\/srv\/daemon-data",
    "sftp": {
      "bind_port": 2022
    }
  },
  "remote": "https:\/\/pterodactyl.file.properties"
}
```
{% endtab %}
{% endtabs %}
