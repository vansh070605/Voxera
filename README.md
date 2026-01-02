# 🎧 Voxera — Real-Time Internet Voice Calling Platform

Voxera is a real-time, internet-based voice calling platform that enables users to communicate instantly over the web.
It uses **WebRTC** for low-latency peer-to-peer audio streaming and **WebSockets (Socket.IO)** for real-time signaling and user presence — similar to how Discord voice chat works.

---

## 🚀 Features

* 🔐 User login with username
* 👥 Real-time online user presence
* 📞 One-to-one voice calling over the internet
* 🎤 Mute / Unmute microphone
* ❌ End call functionality
* 🔄 Peer-to-peer audio streaming (no server audio relay)
* ⚡ Low latency and real-time communication

---

## 🛠️ Tech Stack

### Frontend

* HTML
* CSS
* JavaScript
* WebRTC (audio streaming)
* Socket.IO (client)

### Backend

* Node.js
* Express.js
* Socket.IO (WebSockets)
* STUN server (Google STUN)

---

## 🧠 System Architecture

* **WebSockets** are used for:

  * User login
  * Online/offline presence
  * Call requests
  * WebRTC signaling (SDP & ICE exchange)

* **WebRTC** is used for:

  * Capturing microphone audio
  * Peer-to-peer audio transmission
  * Low-latency voice communication

> ⚠️ Audio data does **not** pass through the server — it flows directly between users.

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
    └── main.js
```

---

## ▶️ How to Run the Project

### 1️⃣ Clone the repository

```bash
git clone https://github.com/vansh070605/Voxera.git
cd Voxera
```

### 2️⃣ Start the backend server

```bash
cd backend
npm install
node server.js
```

You should see:

```
Voxera signaling server running on port 3000
```

### 3️⃣ Run the frontend

* Open `frontend/index.html` in **two browser tabs**
* Login with different usernames
* Click 📞 to start a call

> 💡 Use **Google Chrome** for best WebRTC support.

---

## 🎯 Usage Flow

1. User logs in with a username
2. Online users appear in real time
3. Click 📞 next to a user to initiate a call
4. Receiver accepts the call
5. Audio streams peer-to-peer
6. Use 🔇 Mute or ❌ End Call controls

---

## 🧪 Key Learning Outcomes

* Understanding of **WebRTC architecture**
* Real-time communication using **WebSockets**
* Peer-to-peer media streaming
* ICE candidate exchange and NAT traversal
* Managing call states and media lifecycle
* Building Discord-like VoIP systems from scratch

---

## 🔒 Limitations

* Supports only **1-to-1 voice calls**
* No TURN server (may fail on strict NATs)
* No authentication or encryption layer (demo-level)
* No group calls (yet)

---

## 🚀 Future Enhancements

* 👥 Group voice rooms (Discord-style channels)
* 🎥 Video calling
* 🌍 TURN server integration
* 📊 Network quality indicator
* 🎨 Advanced UI & animations
* 🔐 User authentication

---

## 📄 Project Statement (For Resume)

> **Voxera** is a real-time VoIP web application built using WebRTC and WebSockets that enables low-latency peer-to-peer voice communication with live user presence and call controls.

---

## 👨‍💻 Author

**Vansh Agrawal**
Engineering Student | Web & Real-Time Systems Enthusiast

---

## ⭐ Final Note

This project focuses on **core real-time communication engineering**, not UI gimmicks.
It demonstrates industry-level concepts used in applications like Discord, Zoom, and Google Meet.

---

If you want, next I can:

* ✨ Shorten this README for recruiters
* 📄 Convert it into **project report**
* 🎓 Write **problem statement & abstract**
* 🚀 Prepare **GitHub description + tags**

Just tell me 👌
