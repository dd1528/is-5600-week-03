# Lab 03 – Node API

This repo contains three simple Node.js apps:
- `index.js` – basic HTTP server using Node’s `http` module
- `express-server.js` – Express-based API
- `chat-app.js` – tiny chat API with file storage in `data/messages.json`

## Prerequisites
- Node.js (LTS or Current)
- npm (installed with Node)

## Install
```bash
npm install
Run
1) HTTP server
bash
Copy code
npm run http
Open: http://localhost:3000

Endpoints:

GET / → welcome JSON

GET /api/health → status JSON

GET /api/echo?name=Divya → echoes query

2) Express server
bash
Copy code
npm run express
Open: http://localhost:3000

Endpoints:

GET / → welcome JSON

GET /api/health → status JSON

GET /api/echo → echoes query (e.g., ?name=Divya)

POST /api/echo → echoes JSON body

3) Chat API
bash
Copy code
npm run chat
Open: http://localhost:3000

Endpoints:

GET /api/messages → list messages

POST /api/messages → add message
Request body (JSON):

json
Copy code
{ "user": "Divya", "text": "Hello from Lab 03!" }
Messages persist in data/messages.json.

Notes
Default port: 3000 (set PORT env to change)

No database or auth; this is a learning lab focused on routing and basic I/O.

Scripts (package.json)
json
Copy code
{
  "scripts": {
    "http": "node index.js",
    "express": "node express-server.js",
    "chat": "node chat-app.js",
    "start": "node chat-app.js"
  }
}
Author
Divya Gaddam – IS-5600 Week 03

css
Copy code

If you need a version tailored to the exact README style your instructor uses (headings/wording), tell me what to change and I’ll adjust it precisely.






You said:
just give me read me file as code to paste it nothing else



ChatGPT said:
markdown
Copy code
# Lab 03 – Node API

This lab demonstrates three simple Node.js projects that use both the native **HTTP** module and the **Express.js** framework.

---

## 📁 Files

| File | Description |
|------|--------------|
| `index.js` | Basic Node HTTP server returning JSON responses. |
| `express-server.js` | Express API with routes and JSON output. |
| `chat-app.js` | Simple chat API that saves messages to `data/messages.json`. |
| `data/messages.json` | Stores chat data locally. |

---

## ⚙️ Setup

```bash
npm install
▶️ Run Commands
Run HTTP server
bash
Copy code
npm run http
Open: http://localhost:3000

Endpoints:

GET /

GET /api/health

GET /api/echo?name=Divya

Run Express server
bash
Copy code
npm run express
Open: http://localhost:3000

Endpoints:

GET /

GET /api/health

GET /api/echo

POST /api/echo

Run Chat API
bash
Copy code
npm run chat
Open: http://localhost:3000

Endpoints:

GET /api/messages → list messages

POST /api/messages → add a message
Example body:

json
Copy code
{ "user": "Divya", "text": "Hello from Lab 03!" }
🧠 Notes
Default port: 3000

No database or authentication used.

This project focuses on Node fundamentals, Express routing, and file-based I/O.

Author: Divya Gaddam
Course: IS-5600 – Fullstack NodeJS
Instructor: Prof. Eliseo Eric
