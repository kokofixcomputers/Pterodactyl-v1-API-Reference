# Download Backup

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/backups/<backup uuid>/download`

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/backups/<backup uuid>/download`

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
    "url": "https:\/\/pterodactyl.file.properties:8080\/download\/backup?token=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiIsImp0aSI6IjdkYzAxNzVjODU4MTE5MDRlMjJjNTcxNjBhMjkwMjgwZGFjMDMzM2I2ZmJhMTE3YTI4YjdhMDM5Y2U1OTg0YzcifQ.eyJpc3MiOiJodHRwczpcL1wvcHRlcm9kYWN0eWwuZmlsZS5wcm9wZXJ0aWVzIiwiYXVkIjoiaHR0cHM6XC9cL3B0ZXJvZGFjdHlsLmZpbGUucHJvcGVydGllczo4MDgwIiwianRpIjoiN2RjMDE3NWM4NTgxMTkwNGUyMmM1NzE2MGEyOTAyODBkYWMwMzMzYjZmYmExMTdhMjhiN2EwMzljZTU5ODRjNyIsImlhdCI6MTU5NTE3MjEyNSwibmJmIjoxNTk1MTcxODI1LCJleHAiOjE1OTUxNzMwMjUsImJhY2t1cF91dWlkIjoiOTA0ZGYxMjAtYTY2Zi00Mzc1LWE0YWUtNDBlZWRiZWFlNjMwIiwic2VydmVyX3V1aWQiOiIxYTdjZTk5Ny0yNTliLTQ1MmUtOGI0ZS1jZWNjNDY0MTQyY2EiLCJ1bmlxdWVfaWQiOiJKN1lIQUFUZzVoYVg4M1VOIn0.0zSozCFyjsYjGjUiPS76wM1WXX09FecNxdSZnj6rNt4"
  }
}
```
{% endtab %}
{% endtabs %}
