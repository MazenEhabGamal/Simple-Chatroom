Perfect — here’s your **final reorganized and unique version** of the report, now including a dedicated section for your project video link.
You can simply paste your YouTube or demo link there when it’s ready:

---

# 💬 Go RPC Chatroom System

### 📘 Introduction

The **Go RPC Chatroom** is a lightweight and educational project built in **Go**, designed to demonstrate how **Remote Procedure Calls (RPC)** work using Go’s `net/rpc` package.
It provides a practical example of how multiple clients can communicate with a central server in a distributed environment, showcasing the fundamentals of client-server communication and concurrency in Go.

---

### 🧩 System Structure

This application consists of two main components:

1. **Server (`server.go`)**

   * Runs an RPC service (`HelloService`) that manages incoming client connections and message handling.
   * Stores chat messages in memory and distributes the updated chat log to all connected users.

2. **Client (`client.go`)**

   * Connects to the RPC server through TCP.
   * Sends user input (messages or names) and displays server responses dynamically.

Together, they create a small-scale, interactive chatroom powered entirely by RPC communication.

---

### ⚙️ Core Features

* 🛰️ **RPC-Based Communication** – Built using Go’s native `net/rpc` package for seamless remote method calls.
* 💬 **Interactive Chatting** – Enables users to send and receive messages in real time.
* 🔄 **Concurrent Client Support** – Uses **goroutines** to handle multiple users simultaneously.
* 🧱 **Modular & Extensible** – Can be easily expanded into a full-featured chat system with user authentication, broadcasting, or persistent storage.

---

### 🚀 Running the Application

#### Step 1: Start the Server

Run the following command in your terminal:

```bash
go run server.go
```

You should see:

```
Chat server running on port 1234...
Type 'exit' to stop the server or 'clear' to clear the chat history.
```

#### Step 2: Run the Client

Open another terminal and execute:

```bash
go run client.go
```

Enter your name when prompted and begin chatting 💬
You can open multiple clients at the same time to simulate multiple users interacting in the same chatroom.

---

### 🧠 How It Works

1. Each client connects to the RPC server using a remote method call.
2. Messages are sent in the form of structured data (`ChatMessage` objects).
3. The server stores all chat messages and broadcasts the updated conversation history to every connected client.

This mechanism demonstrates distributed communication through a simple and concurrent design.

---

### 🎥 Project Demonstration

A full walkthrough video of the **Go RPC Chatroom** is available here:
👉 **[Watch the Demo Video]([PASTE-YOUR-LINK-HERE](https://drive.google.com/file/d/1IvaWIaZOZgD7d2hqHDJvJe6bwSW29v1w/view?usp=drive_link))**

The video explains how the project was built, how the communication between server and clients works, and includes a live demonstration of multiple users chatting in real time.

---

### 🧩 Conclusion

The Go RPC Chatroom project provides a hands-on approach to understanding **RPC architecture, concurrency, and client-server design** in Go.
Its clear structure and modular implementation make it an excellent foundation for building more advanced distributed systems and real-time applications.

---

Would you like me to format this as a **clean PDF report** (with title page, sections, and your name/project info) so you can submit it or attach it with your demo link?
