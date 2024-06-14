# Gateway

> **Gateway URL** <br>
> You can view the instant presence of a user with the gateway
> ```
> wss://linkgames.de/api/wss?u={user_id}
> ```

## Payload

```json
{
    "op": 0, // number
    "d": {}, // data
    "t": "" // string
}
```

## Op Codes

| Code | Name          | Description                                             |
|------|---------------|---------------------------------------------------------|
| `0`  | `UPDATE_USER` | `Dispatched when user information or presence changes.` |
| `1`  | `FETCH_USER`  | `Dispatched when connected to the gateway.`             |

## Heartbeat

> The socket connection is pinged every 10 seconds, if the socket does <br> 
> not respond, the connection is terminated. (Socket answers automatically.)

## Example
```js
const ws = new WebSocket('wss://linkgames.de/api/wss?u=954851027188842526');

ws.onmessage = event => {
    try {
        const payload = JSON.parse(event.data);
        if (![ 0, 1 ].includes(payload.op)) return;
        if (![ 'FETCH_USER', 'UPDATE_USER' ].includes(payload.t)) return;
        console.log('user updated: 954851027188842526', payload.d);
    } catch {};
};

/*
user updated: 954851027188842526 {
  "op": 0,
  "t": "UPDATE_USER",
  "d": {
    "id": "954851027188842526",
    "username": "nilscrafthd_",
    "discriminator": "0",
    "tag": "NilsCraftHD",
    "avatar": "208d25844a7a1af4612eda5892181693",
    "avatar_url": "https://cdn.discordapp.com/avatars/954851027188842526/208d25844a7a1af4612eda5892181693.webp",
    "default_avatar": "https://cdn.discordapp.com/embed/avatars/0.png",
    "flags": 256,
    "status": "offline",
    "clients": {},
    "activities": []
  }
}
*/
```