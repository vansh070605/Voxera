````md
<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=34&duration=3000&color=38BDF8&center=true&vCenter=true&width=700&lines=Voxera;Real-Time+Voice+%26+Video+Calling;WebRTC+%7C+Socket.IO;Built+for+Seamless+Communication" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/WebRTC-RealTime-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Socket.IO-WebSockets-black?style=for-the-badge">
  <img src="https://img.shields.io/badge/Node.js-Backend-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
</p>

---

# 🎧 Voxera — Real-Time Voice, Video & Screen Sharing Platform

> **Voxera** is a browser-based real-time communication platform that enables **low-latency voice calls, video calls, and screen sharing** using modern web technologies.

Inspired by platforms like **Google Meet** and **Discord Voice**, Voxera focuses on **core real-time communication engineering**, not just UI demos.

---

## ✨ Live Preview (Add Later)

> 📌 *You can add GIFs/screenshots here once deployed*

```text
📸 Login Screen → 📞 Call Initiation → 🎥 Video Call → 🖥️ Screen Sharing
````

<p align="center">
  <img src="https://user-images.githubusercontent.com/placeholder/login.gif" width="80%" />
</p>

---

## 🚀 Features at a Glance

### 🔗 Real-Time Communication

* 📞 One-to-one voice & video calls
* 🖥️ Screen sharing with system audio
* ⚡ Ultra-low latency (P2P WebRTC)
* 🔊 Call connect / end sound effects
* ❌ Synchronized call ending (both users disconnect)

### 🎛 Call Controls

* 🎤 Mute / Unmute microphone
* 🖥️ Start / Stop screen sharing
* 📞 End call
* 🪟 Floating camera (PiP mode)

### 🎨 UI & Experience

* ✨ Google Meet–inspired interface
* 🌌 Glassmorphism & gradient background
* 🎥 Smart video layout (screen-first)
* 🔔 Call status overlays (Calling / Incoming)
* 🎧 Idle onboarding screen

---

## 🛠️ Tech Stack

### 🖥️ Frontend

* HTML5
* CSS3 (Glassmorphism + Animations)
* JavaScript (ES6+)
* WebRTC (Audio, Video, Screen Capture)
* Socket.IO Client

### ⚙️ Backend

* Node.js
* Express.js
* Socket.IO (WebSockets)
* Google STUN Server

---

## 🧠 Architecture Overview

```text
User A  ── WebRTC (Audio/Video/Screen) ──▶  User B
   │                                         ▲
   └── Socket.IO (Signaling & Presence) ─────┘
```

### 🔄 WebSockets Handle:

* User login & presence
* Online user list
* Call requests
* SDP & ICE signaling
* Call end synchronization

### 🎥 WebRTC Handles:

* Peer-to-peer media streaming
* Microphone & camera capture
* Screen sharing
* NAT traversal (ICE)

> ⚠️ Media streams **never pass through the server**

---

## 📁 Project Structure

```
Voxera/
│
├── backend/
│   ├── server.js
│   └── package.json
│
└── frontend/
    ├── index.html
    ├── style.css
    ├── main.js
    └── sounds/
        ├── call-connect.mp3
        ├── screen-share.mp3
        └── call-end.mp3
```

---

## ▶️ How to Run

### 1️⃣ Clone Repository

```bash
git clone https://github.com/vansh070605/Voxera.git
cd Voxera
```

### 2️⃣ Start Backend

```bash
cd backend
npm install
node server.js
```

```text
✅ Voxera signaling server running on port 3000
```

### 3️⃣ Start Frontend

* Open `frontend/index.html` in **two browser tabs**
* Login with different usernames
* Start calling 🚀

> 💡 Best experience on **Google Chrome**

---

## 🎯 Call Flow (Step-by-Step)

```text
Login → Online Users → Call → Connect → Share Screen → End Call
```

✔ Ending call on one side **disconnects both users**
✔ UI resets cleanly on both ends

---

## 🧪 What This Project Demonstrates

* WebRTC internals & signaling
* ICE candidate exchange
* Media track replacement (screen share)
* Real-time state synchronization
* Peer-to-peer networking
* Production-style UI & UX

---

## 🔒 Current Limitations

* 🔹 One-to-one calls only
* 🔹 No TURN server
* 🔹 No authentication system
* 🔹 No recording support
* 🔹 No group calls (yet)

---

## 🚀 Future Enhancements

* 👥 Group calls / voice rooms
* 🎥 Camera toggle
* ⏱️ Call duration timer
* 🔐 User authentication
* 🌍 TURN server support
* 📊 Network quality metrics
* 📱 Mobile-first UI

---

## 📄 Resume-Ready Project Statement

> **Voxera** is a real-time communication web application built using WebRTC and WebSockets that enables peer-to-peer voice calls, video calls, and screen sharing with synchronized call lifecycle management and a modern production-grade UI.

---

## 👨‍💻 Author

**Vansh Agrawal**
Engineering Student | Full-Stack & Real-Time Systems Enthusiast

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=vansh070605&show_icons=true&theme=tokyonight" />
</p>

---

## ⭐ Final Words

This project showcases **real-world communication engineering** used in platforms like
**Google Meet, Zoom, and Discord** — built completely from scratch.

---
