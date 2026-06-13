## Project Structure
├── Message.java          # Serializable message object sent over the network
├── WhiteboardServer.java  # Server that accepts client connections and broadcasts drawing events
└── WhiteboardClient.java  # Swing GUI client for drawing on the whiteboard

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
