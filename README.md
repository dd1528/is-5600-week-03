# Lab 03 – Node API (HTTP, Express, Chat)

This lab demonstrates how to build and test Node.js web servers using the **HTTP module** and **Express.js** framework.  
It includes three parts: a basic HTTP server, an Express API, and a mini chat service with file-based persistence.

---

## 🧩 Project Files

| File | Description |
|------|--------------|
| `index.js` | Basic Node.js HTTP server that responds with simple messages. |
| `express-server.js` | Express API that returns structured JSON responses. |
| `chat-app.js` | Chat API built with Express that reads/writes messages from `data/messages.json`. |
| `data/messages.json` | Stores all chat messages locally in JSON format. |

---

## ⚙️ Setup Instructions

1. Clone this repository or open it in **VS Code**.  
2. Install dependencies:
   ```bash
   npm install
