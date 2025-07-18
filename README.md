# 🏛️ SmartGov – Digital Civic Issue Tracker

A full-stack web platform that helps **citizens report public issues** (like potholes, broken street lights, sewage leaks), and allows **government officials to track, assign, and resolve** them. Built with a powerful **role-based access control (RBAC)** system, real-time alerts, geo-tagging, and analytics.

## 👥 Roles & Access

| Role            | Permissions                                                                 |
|-----------------|------------------------------------------------------------------------------|
| **Citizen**     | Create issues, upload images, track issue status, view public board         |
| **Officer**     | View assigned issues, update resolution status, manage issue lifecycle       |
| **Admin**       | Manage departments, assign officers, view area-wise analytics, dashboard     |

## 💡 Features

- 📍 **Map-Based Reporting** (Leaflet + Location API)
- 🖼️ **Image Uploads** (evidence support with Multer + MongoDB)
- 🔐 **RBAC**: Protected routes & features based on user role
- 📊 **Admin Analytics**: Area-wise issue count, department performance
- 🧾 **Public Transparency Board**: View resolved and pending issues

---

## 🛠️ Tech Stack

| Layer       | Technology                                                  |
| ----------- | ----------------------------------------------------------- |
| 🌐 Frontend | React.js, Tailwind CSS, TypeScript, Zustand, TanStack Query |
| 🖥 Backend  | Node.js, Express.js                                         |
| 🗄 Database | MongoDB                                                     |
| 📡 Realtime | Socket.IO                                                   |
| 🔐 Auth     | JWT & Bcrypt                                                |
| 🧠 Logic    | MongoDB Aggregation Pipelines                               |
| 📍 Location | MongoDB Geospatial Queries                                  |



## 📦 Setup Instructions

### 1. Fork the Repository
Go to [CivicSync Repository]([https://github.com/kotlalokeshwari098/CivicSync]) and click the **Fork** button in the top-right corner to create a copy under your GitHub account.

### 2. Clone Your Forked Repository
```bash
git clone https://github.com/<your-username>/CivicSync.git
NOTE:Replace <your-username> with your actual GitHub username.
cd CivicSync
```
### 3. Install Server Dependencies
```bash
cd server
npm install
```
### 4. Install Client Dependencies
```bash
cd client
npm install
```
### 5. Set Up Environment Variables
Create a .env file in the server directory with the following:
```bash
PORT=5000
DB_CONNECT=your-db-connection
JWT_SECRET=your_jwt_secret_here

# Optional external geolocation APIs
NOMINATIM_MAPS=https://example.com/nominatim/search
PHOTON_URL=https://example.com/photon/api
```
### 6. Run the Server
```bash
cd server
npm run dev
```
### 7. Run the Client
```bash
cd client
npm run dev
```
---

⚠️ This is a personal project and is not open for external contributions at the moment.
