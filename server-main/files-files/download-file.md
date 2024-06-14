# Download File

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/contents?file=paper.yml`

## Get Server Details

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/files/contents?file=paper.yml`

**Parameters**

| Name   | Description               |
| ------ | ------------------------- |
| `file` | file to view content from |

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
  "object": "signed_url",
  "attributes": {
    "url": "https:\/\/pterodactyl.file.properties:8080\/download\/file?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6IjdkYzAxNzVjODU4MTE5MDRlMjJjNTcxNjBhMjkwMjgwZGFjMDMzM2I2ZmJhMTE3YTI4YjdhMDM5Y2U1OTg0YzcifQ.eyJpc3MiOiJodHRwczpcL1wvcHRlcm9kYWN0eWwuZmlsZS5wcm9wZXJ0aWVzIiwiYXVkIjoiaHR0cHM6XC9cL3B0ZXJvZGFjdHlsLmZpbGUucHJvcGVydGllczo4MDgwIiwianRpIjoiN2RjMDE3NWM4NTgxMTkwNGUyMmM1NzE2MGEyOTAyODBkYWMwMzMzYjZmYmExMTdhMjhiN2EwMzljZTU5ODRjNyIsImlhdCI6MTU5NDY0ODEwMCwibmJmIjoxNTk0NjQ3ODAwLCJleHAiOjE1OTQ2NDkwMDAsImZpbGVfcGF0aCI6IlwvZXVsYS50eHQiLCJzZXJ2ZXJfdXVpZCI6IjFhN2NlOTk3LTI1OWItNDUyZS04YjRlLWNlY2M0NjQxNDJjYSIsInVuaXF1ZV9pZCI6IlNvWUdIamNaNmhKUVlieHUifQ.h4eBmxDXf-4GAwVuAWZFU5QTqd62jw7HTre4aKQGpvw"
  }
}
```
{% endtab %}
{% endtabs %}
