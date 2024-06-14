# Websocket



## Connect to websocket after getting credentials [generates-websocket-credentials.md](server-main/generates-websocket-credentials.md "mention")

<mark style="color:green;">`WSS`</mark> `wss://pterodactyl/api/servers/<Server UUID>/ws`

**Messages to send:**

**Authenticate:**

Use the token you got from [generates-websocket-credentials.md](server-main/generates-websocket-credentials.md "mention") as args

`{"event":"auth","args":["<token>"]}`

**Get Status:**

`{"event":"send stats","args":[null]}`

**Get Logs:**

`{"event":"send logs","args":[null]}`

**Send Power Action:**

`{"event":"set state","args":["<kill/start/restart/stop>"]}`

**Send an Command:**

`{"event":"send command","args":["<command>"]}`
