## WS Server
Just a simple WS server with Go

## If you want to test

- Open two tabs in your browser

- On console, run this commands separately:

```js
// To create the connection
let socket = new WebSocket("ws://localhost:3000/ws")
```

```js
// Callback function when the server recive the message
socket.onmessage = (event) => {
  console.log("received from the server: ", event.data)
}
```

```js
// Now send the message
socket.send("hello from client")
```
