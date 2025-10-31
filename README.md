Here’s a rewritten version of your report with fresh phrasing and structure — it keeps the same meaning but reads as your own unique work:

---

## 💬 Go RPC Chatroom

This project is a lightweight chatroom built in **Go**, designed to showcase the core principles of **Remote Procedure Call (RPC)** communication using Go’s built-in `net/rpc` package.
It provides a simple yet powerful demonstration of how clients and a central server can exchange data through remote function calls. [Watch the demo here.]

---

## 🧠 Overview

The system is composed of two main files:

| File          | Purpose                                                                                  |
| ------------- | ---------------------------------------------------------------------------------------- |
| **server.go** | Runs the RPC service (`HelloService`), managing client connections and message handling. |
| **client.go** | Connects to the RPC server, sends chat inputs, and receives the server’s responses.      |

Communication happens over **TCP**, where each client interacts with the server via remote method calls — forming the backbone of a distributed chat environment.

---

## ⚙️ Key Features

* 🛰️ **RPC Communication** – Implements a clear request/response workflow using Go’s `net/rpc` library.
* 💬 **Interactive Chatting** – Clients can send their messages or names and get real-time responses.
* 🔄 **Multi-Client Support** – Handles multiple users simultaneously through **goroutines**.
* 🔧 **Scalable Structure** – Easily adaptable into a complete chat system with broadcasting or message storage.

---

## 🏗️ Running the Project

### 1️⃣ Launch the Server

```bash
go run server.go
```

Expected output:

```
💬 Chat server active on port 1234...
Type 'exit' to stop the server or 'clear' to reset chat history.
```

### 2️⃣ Start the Client

In a separate terminal window:

```bash
go run client.go
```

Enter your name when prompted, then begin chatting 💬
You can open multiple clients to simulate a multi-user chat session.

---

## 🧠 Behind the Scenes

* The server maintains a simple in-memory chat history.
* Each connected client sends messages (via `ChatMessage` structs) through RPC calls.
* The server records new messages and returns the updated conversation log to all clients in real time.

---

Would you like me to make it sound a bit **more formal and technical** (like a report for a course submission) or **more casual and readable** (like a GitHub README)?
