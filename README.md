# Distributed-Shared-White-Board
A networked **shared whiteboard** that allows multiple users to draw and collaborate on the same canvas in real time.  
The first user starts the session as the **manager** (server/host). Other users join as **peers** (clients). The manager approves join requests and can manage the session.

## Repository Contents

- `CreateWhiteBoard.jar` — Launches the whiteboard as the **manager/host** (server).
- `JoinWhiteBoard.jar` — Launches the whiteboard as a **peer/client** to join an existing session.
- `demo.png` — Screenshot showing the application UI and synchronized drawing result.
- `Project2-Sem1-2024.pdf` — Assignment specification / requirements document.
- `Project_Report.pdf` — Project report describing design, implementation, and testing.
- `design diagram.pdf` — System design diagrams (e.g., architecture / class / sequence diagrams).
- `source code.zip` — Source code archive for the project.
- `README.md` — Project overview and usage instructions.


## Demo
![Distributed Whiteboard Demo](./demo.png)

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

