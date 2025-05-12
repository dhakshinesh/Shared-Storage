# 🖥️ Collaborative Storage Pool (Desktop-First)

A **decentralized, multi-user file-sharing platform** built around a Tkinter desktop application.  
Users who trust each other can **join a shared storage pool**, contribute their device's local storage, and **collaborate on files in real time**.

> 🎯 Focus: **Python + Tkinter Desktop App**  
> 🌐 Backend: Django REST API  
> 🧩 Frontend (optional): Vue.js Web Dashboard

---

## 💡 Concept

Unlike cloud storage services like Google Drive or Dropbox, this project aims to:
- **Avoid centralized hosting**
- **Use users' devices as storage nodes**
- Enable real-time sync and collaboration
- Support offline access with automatic sync on reconnect

Users form **storage pools** with an ID & password, share files with each other, and all data is handled peer-to-peer.

---

## 🧠 Key Modules (Open to Contributors)

### 🖥️ 1. Tkinter Desktop App (Primary Focus)
- Login/Join storage pool (ID + password)
- Dashboard UI (file list, upload, download, delete)
- Multi-threading support for smooth file transfer
- Live notifications for file updates
- Caching files locally for offline access
- Real-time sync (sockets or polling)
- Configurable settings per user

### 🌐 2. Django Backend (API Server)
- REST endpoints for:
  - Authentication
  - Pool creation/joining
  - File metadata exchange
- WebSocket (or fallback polling) for real-time updates
- Storage indexing and conflict resolution logic

### 🧪 3. Data Management & Sync Logic
- Chunked file transfer
- File encryption/decryption
- Peer discovery (via backend or broadcast)
- File locking and versioning

---

## ⚙️ Tech Stack

| Component     | Technology          |
|---------------|---------------------|
| Desktop UI    | **Python Tkinter**  |
| Backend API   | Django + DRF        |
| Real-Time     | WebSocket / Polling |
| Frontend (opt)| Vue 3               |
| Storage Format| Local Filesystem    |

---

## 🔐 Security & Privacy

- Password-protected storage pools
- Local encryption of files before transfer
- Role-based access control (Admin/Contributor)
- No central file storage – all user-owned

---

## 🚀 Getting Started

> 🧩 Full setup instructions are in [`docs/setup.md`](docs/setup.md) (coming soon)

### 1. Clone the Repo
```bash
git clone https://github.com/your-username/storage-pool.git
cd storage-pool
