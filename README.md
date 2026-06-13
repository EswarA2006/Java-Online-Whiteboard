# Java Online Whiteboard 🎨

A simple real-time collaborative whiteboard built with Java Swing and sockets.
Multiple clients can connect to a server and draw together on a shared canvas.

## Project Structure

```
.
├── Message.java          # Serializable message object sent over the network
├── WhiteboardServer.java  # Server that accepts client connections and broadcasts drawing events
└── WhiteboardClient.java  # Swing GUI client for drawing on the whiteboard
```

## Requirements

- Java JDK 8 or later

## How to Run

1. Compile all files:
   ```bash
   javac *.java
   ```

2. Start the server (run this once, on the host machine):
   ```bash
   java WhiteboardServer
   ```

3. Start one or more clients (run on the host machine or any machine on the same network):
   ```bash
   java WhiteboardClient <server-ip>
   ```
   Replace `<server-ip>` with the server machine's IP address (use `localhost` if running on the same machine).

4. Draw on the canvas in any client window — your strokes will appear in real time on all connected clients.

## Notes

- The server listens on port `5000` by default.
- Make sure that port is open/forwarded if connecting across different networks.

## License

This project is open source — feel free to use and modify it.
