# -Distributed-Shared-White-Board
A networked **shared whiteboard** that allows multiple users to draw and collaborate on the same canvas in real time.  
The first user starts the session as the **manager** (server/host). Other users join as **peers** (clients). The manager approves join requests and can manage the session.

## Key Features
- Real-time shared canvas (all users see the same whiteboard state)
- Drawing tools: freehand draw, eraser
- Shapes: line, rectangle, circle/oval
- Text tool (type anywhere on the board)
- Colour palette (multiple colours)
- Online user list (see who is currently connected)
- Manager controls: approve join requests, manage/remove peers, and session lifecycle

- 
## Getting Started
- ### Prerequisites
- Java (JRE/JDK) installed  
  Check with:
  ```bash
  java -version
  ```
  
## Run the Application (2 JARs)

### 1) Start the whiteboard as **Manager** (creates/hosts the session)

```bash
java -jar CreateWhiteBoard.jar <serverIPAddress> <serverPort> <username>
```

### 2) Start the whiteboard as **client** (creates/hosts the session)

```bash
java -jar JoinWhiteBoard.jar <serverIPAddress> <serverPort> <username>
```

