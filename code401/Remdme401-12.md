# Socket.IO

Socket.IO is a library that enables real-time, bidirectional and event-based communication between the browser and the server.

## How does that work?

The client will try to establish a WebSocket connection if possible, and will fall back on HTTP long polling if not.

WebSocket is a communication protocol which provides a full-duplex and low-latency channel between the server and the browser.

const socket = io("ws://localhost:3000");

socket.on("connect", () => {
  // either with send()
  socket.send("Hello!");

  // or with emit() and custom event names
  socket.emit("salutations", "Hello!", { "mr": "john" }, Uint8Array.from([1, 2, 3, 4]));
});

// handle the event sent with socket.send()
socket.on("message", data => {
  console.log(data);
});

// handle the event sent with socket.emit()
socket.on("greetings", (elem1, elem2, elem3) => {
  console.log(elem1, elem2, elem3);
});

## What Socket.IO is not

Socket.IO is NOT a WebSocket implementation. Although Socket.IO indeed uses WebSocket as a transport when possible, it adds additional metadata to each packet.

## philosophy from me

this is a package from the node.js, you can require it in the app when you want to use it and it makes the browser like life.

example: chat app
let's say you create a chat app and you open a browser with 3 tabs and this tab reference the app, and when you send a message from any tab it will appear in the another tab.
if you make for the app page for the sign in and this sign-in will send some information in the database and you return from it the user name and used in the app for when any user sends a message it will appear with the name user and also you can add date for know when this message it sends.