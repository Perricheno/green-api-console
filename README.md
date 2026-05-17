<div align="center">

<img src="https://img.shields.io/badge/GREEN--API-WhatsApp-25d366?style=for-the-badge&logo=whatsapp&logoColor=white" />
<img src="https://img.shields.io/badge/HTML5-Single--Page-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
<img src="https://img.shields.io/badge/Node.js-Server-339933?style=for-the-badge&logo=nodedotjs&logoColor=white" />
<img src="https://img.shields.io/badge/License-MIT-blue?style=for-the-badge" />

# 💬 GREEN-API · WhatsApp Instance Console

**A GitHub-styled single-page application for managing your WhatsApp instance via [GREEN-API](https://green-api.com).**  
Send messages, files, and inspect your instance — all from a clean dark-mode UI.

<!-- СКРИН -->
> 📸 _Screenshot coming soon_
<!-- СКРИН -->

[**🌐 Live Demo**](https://test.perricheno.ru) · [**📖 GREEN-API Docs**](https://green-api.com/docs) · [**🐛 Report Bug**](https://github.com/Perricheno/green-api-console/issues)

</div>

---

## ✨ Features

- **4 API methods** — `getSettings`, `getStateInstance`, `sendMessage`, `sendFileByUrl`
- **Syntax-highlighted JSON** responses with HTTP status badges
- **Request history** — browse past calls with timestamps and status indicators
- **Live connection status** — real-time instance state in the navbar
- **Auto-detected API URL** — paste your `idInstance` and the URL fills itself
- **Copy / Clear** — one-click copy of any response to clipboard
- **GitHub dark theme** — fully responsive, no external dependencies

---

## 🖼️ Interface

| Panel | Description |
|---|---|
| **Left** | Credentials, API method buttons, message/file inputs |
| **Right** | JSON response viewer, request history tab |

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/Perricheno/green-api-console.git
cd green-api-console
```

### 2. Run the server

```bash
node server.js
# → http://localhost:3545
```

> Requires **Node.js 14+**. No dependencies to install — pure standard library.

### 3. Open in browser

Navigate to `http://localhost:3545` and enter your GREEN-API credentials.

---

## 🔑 How to Get Credentials

1. Register a free developer account at [console.green-api.com](https://console.green-api.com)
2. Create a new instance → scan the QR code with WhatsApp
3. Copy `idInstance` and `ApiTokenInstance` from the instance dashboard
4. Paste them into the console and hit **Test Connection**

---

## 📡 API Methods

| Method | Type | Description |
|---|---|---|
| `getSettings` | `GET` | Retrieve all current instance settings |
| `getStateInstance` | `GET` | Check authorization state of the instance |
| `sendMessage` | `POST` | Send a text message to a phone number or group |
| `sendFileByUrl` | `POST` | Send an image, video, or document via URL |

### Chat ID format

| Type | Format | Example |
|---|---|---|
| Personal chat | `{phone}@c.us` | `77001234567@c.us` |
| Group chat | `{id}@g.us` | `120363043968066561@g.us` |

---

## 🛠️ Tech Stack

- **Frontend** — Vanilla HTML/CSS/JS (zero frameworks, zero dependencies)
- **Server** — Node.js built-in `http` module
- **Styling** — GitHub Primer design system (hand-crafted)
- **Deployment** — Cloudflare Tunnel → `test.perricheno.ru`

---

## 📁 Project Structure

```
green-api-console/
├── index.html   # Single-page application (all UI + JS)
└── server.js    # Minimal static file server (Node.js)
```

---

## 📄 License

MIT © [Perricheno](https://github.com/Perricheno)

---

<div align="center">
  <sub>Built as a DevOps test assignment for <a href="https://green-api.com">GREEN-API</a></sub>
</div>
