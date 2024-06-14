# List Files

**Request method: GET**

Request Example: `https://pterodactyl/api/client/servers/<Server ID>/files/list? directory=.cache`

## Get Server Details

<mark style="color:green;">`GET`</mark> `/api/client/servers/<Server ID>/files/list?directory=.cache`

**Parameters**

| Name        | Description                       |
| ----------- | --------------------------------- |
| `directory` | Get the files from this directory |

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
      "object": "file_object",
      "attributes": {
        "name": "cache",
        "mode": "drwxr-xr-x",
        "size": 4096,
        "is_file": false,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "inode\/directory",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:20:36+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "logs",
        "mode": "drwxr-xr-x",
        "size": 4096,
        "is_file": false,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "inode\/directory",
        "created_at": "2020-07-13T12:42:02+00:00",
        "modified_at": "2020-07-13T12:42:02+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "plugins",
        "mode": "drwxr-xr-x",
        "size": 4096,
        "is_file": false,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "inode\/directory",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:07+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "world",
        "mode": "drwxr-xr-x",
        "size": 4096,
        "is_file": false,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "inode\/directory",
        "created_at": "2020-07-13T13:26:22+00:00",
        "modified_at": "2020-07-13T13:26:22+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "world_nether",
        "mode": "drwxr-xr-x",
        "size": 4096,
        "is_file": false,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "inode\/directory",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:15+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "world_the_end",
        "mode": "drwxr-xr-x",
        "size": 4096,
        "is_file": false,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "inode\/directory",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:15+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "whitelist.json",
        "mode": "-rw-r--r--",
        "size": 2,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "application\/json",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:07+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "version_history.json",
        "mode": "-rw-r--r--",
        "size": 46,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "application\/json",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:08+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "usercache.json",
        "mode": "-rw-r--r--",
        "size": 2,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "application\/json",
        "created_at": "2020-07-13T12:42:03+00:00",
        "modified_at": "2020-07-13T12:42:03+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "spigot.yml",
        "mode": "-rw-r--r--",
        "size": 3567,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2020-06-12T21:44:42+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "server.properties",
        "mode": "-rw-r--r--",
        "size": 955,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:59+00:00",
        "modified_at": "2020-07-13T12:41:59+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "server.jar",
        "mode": "-rw-r--r--",
        "size": 36175593,
        "is_file": true,
        "is_symlink": false,
        "is_editable": false,
        "mimetype": "application\/jar",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2020-06-12T22:38:46+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "permissions.yml",
        "mode": "-rw-r--r--",
        "size": 0,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "inode\/x-empty",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:08+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "paper.yml",
        "mode": "-rw-r--r--",
        "size": 5310,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2020-06-12T21:44:42+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "ops.json",
        "mode": "-rw-r--r--",
        "size": 2,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "application\/json",
        "created_at": "2020-07-13T12:42:03+00:00",
        "modified_at": "2020-07-13T12:42:03+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "hs_err_pid25.log",
        "mode": "-rw-r--r--",
        "size": 57099,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2020-06-12T20:36:55+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "help.yml",
        "mode": "-rw-r--r--",
        "size": 2576,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:21:07+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "eula.txt",
        "mode": "-rw-r--r--",
        "size": 250,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2019-12-25T05:20:57+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "commands.yml",
        "mode": "-rw-r--r--",
        "size": 598,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2020-06-12T21:44:36+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "bukkit.yml",
        "mode": "-rw-r--r--",
        "size": 1053,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "text\/plain",
        "created_at": "2020-07-13T12:41:55+00:00",
        "modified_at": "2020-06-12T21:44:36+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "banned-players.json",
        "mode": "-rw-r--r--",
        "size": 2,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "application\/json",
        "created_at": "2020-07-13T12:42:03+00:00",
        "modified_at": "2020-07-13T12:42:03+00:00"
      }
    },
    {
      "object": "file_object",
      "attributes": {
        "name": "banned-ips.json",
        "mode": "-rw-r--r--",
        "size": 2,
        "is_file": true,
        "is_symlink": false,
        "is_editable": true,
        "mimetype": "application\/json",
        "created_at": "2020-07-13T12:42:03+00:00",
        "modified_at": "2020-07-13T12:42:03+00:00"
      }
    }
  ]
}
```
{% endtab %}
{% endtabs %}
