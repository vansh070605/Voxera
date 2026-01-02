<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=36&duration=3000&color=38BDF8&center=true&vCenter=true&width=800&lines=Voxera;Real-Time+Voice+Video+%26+Screen+Sharing;WebRTC+%7C+Socket.IO;Built+for+Seamless+Communication" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/WebRTC-Real--Time-blue?style=for-the-badge">
  <img src="https://img.shields.io/badge/Socket.IO-WebSockets-black?style=for-the-badge">
  <img src="https://img.shields.io/badge/Node.js-Backend-green?style=for-the-badge">
  <img src="https://img.shields.io/badge/Status-Active-success?style=for-the-badge">
</p>

---

# 🎧 Voxera — Real-Time Communication Platform

**Voxera** is a browser-based real-time communication platform that enables **low-latency voice calls, video calls, and screen sharing** directly over the internet.

Inspired by platforms like **Google Meet**, **Zoom**, and **Discord Voice**, Voxera focuses on **core real-time communication engineering** using modern web technologies.

---

## ✨ Live Demo Preview (Add Screenshots/GIFs)

```text
Login → Online Users → Call → Video → Screen Share → End Call
````

> 
![Home Page](image.png)

![Call Page](image-1.png)
---

## 🚀 Features

### 🔗 Real-Time Communication

* 📞 One-to-one voice & video calls
* 🖥️ Screen sharing with system audio
* ⚡ Ultra-low latency peer-to-peer streaming
* 🔊 Call connect, screen share & call end sounds
* ❌ Synchronized call ending (ends on both sides)

### 🎛 Call Controls

* 🎤 Mute / Unmute microphone
* 🖥️ Start / Stop screen sharing
* 📞 End call
* 🪟 Floating camera (Picture-in-Picture)

### 🎨 UI & UX

* ✨ Google Meet–inspired professional UI
* 🌌 Glassmorphism + gradient background
* 🎥 Smart video layout (screen-first, camera PiP)
* 🔔 Call status overlays (Calling / Incoming)
* 🎧 Idle onboarding screen

---

## 🛠️ Tech Stack

### 🖥️ Frontend

* HTML5
* CSS3 (Glassmorphism, animations)
* JavaScript (ES6+)
* WebRTC (Audio, Video, Screen Capture)
* Socket.IO (Client)

### ⚙️ Backend

* Node.js
* Express.js
* Socket.IO (WebSockets)
* Google STUN Server

---

## 🧠 Architecture Overview

```text
User A  ── WebRTC (Audio / Video / Screen) ──▶  User B
   │                                             ▲
   └──── Socket.IO (Signaling & Presence) ───────┘
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
* Screen sharing with system audio
* NAT traversal via ICE

> ⚠️ Media streams **do not pass through the server** — they flow directly between peers.

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

## ▶️ How to Run the Project

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/vansh070605/Voxera.git
cd Voxera
```

### 2️⃣ Start the Backend Server

```bash
cd backend
npm install
node server.js
```

Expected output:

```text
✅ Voxera signaling server running on port 3000
```

### 3️⃣ Run the Frontend

* Open `frontend/index.html` in **two browser tabs or devices**
* Login with different usernames
* Start calling 🚀

> 💡 Recommended browser: **Google Chrome**

---

## 🎯 Call Flow

```text
Login → Select User → Call → Connect → Share Screen → End Call
```

✔ Ending a call on one side **disconnects both users**
✔ UI resets cleanly on both ends

---

## 🧪 What This Project Demonstrates

* WebRTC signaling & peer connection setup
* ICE candidate exchange and NAT traversal
* Media track replacement (screen sharing)
* Real-time state synchronization
* Peer-to-peer networking concepts
* Production-style UI & call lifecycle management

---

## 🔒 Current Limitations

* 🔹 One-to-one calls only
* 🔹 No TURN server (may fail on strict NATs)
* 🔹 No authentication system
* 🔹 No call recording
* 🔹 No group calls (yet)

---

## 🚀 Future Enhancements

* 👥 Group calls / voice rooms
* 🎥 Camera on/off toggle
* ⏱️ Call duration timer
* 🔐 User authentication
* 🌍 TURN server integration
* 📊 Network quality indicators
* 📱 Mobile responsiveness

---

## 📄 Resume-Ready Project Statement

> **Voxera** is a real-time communication web application built using WebRTC and WebSockets that enables peer-to-peer voice calls, video calls, and screen sharing with synchronized call lifecycle management and a modern, production-grade UI.

---

## 👨‍💻 Author

**Vansh Agrawal**
Engineering Student | Full-Stack & Real-Time Systems Enthusiast

---

## ⭐ Final Note

Voxera focuses on **real-world real-time communication engineering**, not just UI demos.
It demonstrates the same foundational concepts used in **Google Meet, Zoom, and Discord** — built completely from scratch.

---