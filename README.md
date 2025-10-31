# 💬 Go RPC Chatroom System

### 📘 Introduction

The **Go RPC Chatroom** is a minimal yet instructive project that explores how **Remote Procedure Calls (RPC)** work in Go using the `net/rpc` package.
It provides a working example of how multiple clients can communicate through a single coordinating server, illustrating the basics of distributed systems in a clean and extensible design.

---

### 🧩 System Structure

This application is made up of two core components:

1. **Server (`server.go`)**

   * Hosts an RPC service (`HelloService`) responsible for managing connections and processing messages from clients.
   * Maintains a chat history and returns updates to connected users.

2. **Client (`client.go`)**

   * Connects to the RPC server over TCP.
   * Sends user input to the server and displays the server’s response in real time.

Together, these two programs demonstrate how Go can handle message passing and coordination through RPC communication.

---

### ⚙️ Core Features

* 🛰️ **RPC Messaging System** – Built entirely on Go’s native `net/rpc` for seamless client-server communication.
* 💬 **Interactive Exchange** – Users can send text or identifiers and receive instant replies from the server.
* 🔄 **Concurrent Clients** – Supports multiple connections simultaneously via goroutines, allowing real-time chat interaction.
* 🧱 **Expandable Framework** – Can be extended to include broadcasting, user management, or database-backed message storage.

---

### 🚀 Getting Started

#### Step 1: Run the Server

Execute the following command in your terminal:

```bash
go run server.go
```

You should see a message similar to:

```
Chat server started on port 1234
Type 'exit' to stop the server or 'clear' to reset the chat log.
```

#### Step 2: Launch a Client

Open another terminal window and run:

```bash
go run client.go
```

After entering your name, you can start chatting immediately.
Open several clients at once to simulate multiple participants in the chatroom.

---

### 🧠 Internal Workflow

1. Each client connects to the server through an RPC call.
2. Messages are sent as structured data (`ChatMessage` objects).
3. The server stores all messages in memory and distributes the updated chat history to every active client.

This setup demonstrates the foundation of distributed communication—simple, concurrent, and easily extensible.

---

### 🧩 Summary

The Go RPC Chatroom project is more than just a small app—it’s a **hands-on guide** to understanding RPC concepts in Go.
By separating the client and server logic, it provides a clean example of **request/response-based interaction** and concurrent networking using **goroutines**.
It serves as an excellent starting point for anyone learning about **Go networking, RPC systems, or distributed architecture**.
