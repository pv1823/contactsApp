# 📇 Contacts App - MEAN Stack Contact Manager

![Node.js](https://img.shields.io/badge/Node.js-Express-informational)
![MongoDB](https://img.shields.io/badge/MongoDB-Database-brightgreen)
![Docker](https://img.shields.io/badge/Containerized-Docker-blue)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

A modern web-based contact management system built using the MERN stack (MongoDB, Express.js, Angular, Node.js). It allows users to securely manage contacts with CRUD operations, search filters, and role-based authentication.

---

## 🚀 Features

- ✅ Create, Read, Update, Delete (CRUD) contacts
- ✅ Categorize contacts (e.g., Work, Personal)
- ✅ Smart search with filters
- ✅ Secure authentication using JWT
- ✅ Encrypted data storage
- ✅ Docker-ready backend
- ✅ Deployed on AWS (or ready to be)

---

## 🧱 Tech Stack

| Layer         | Technology                |
|---------------|----------------------------|
| Frontend      | Angular.js (not included here) |
| Backend       | Node.js + Express.js      |
| Database      | MongoDB                   |
| Auth          | JWT + Bcrypt              |
| Container     | Docker                    |
| Deployment    | AWS EC2 (optional)        |

---

## 📁 Folder Structure

```
ContactsApp/
├── controllers/
├── models/
├── routes/
├── middleware/
├── config/
│   └── db.js
├── .env.example
├── Dockerfile
├── package.json
└── README.md
```

---

## 🛠️ Getting Started

### 🔧 Prerequisites

- Node.js 18+
- MongoDB Atlas or local MongoDB
- Docker (optional)

### 🧪 Run Locally

```bash
# Install dependencies
npm install

# Create .env file from template
cp .env.example .env

# Start backend server
node server.js
```

---

### 🐳 Docker Setup

```bash
# Build image
docker build -t contacts-app-backend .

# Run container
docker run -p 5000:5000 --env-file .env contacts-app-backend
```

---

## 🗂️ Environment Variables

Copy `.env.example` and rename to `.env`:

```
PORT=5000
MONGO_URI=mongodb://localhost:27017/contactsdb
JWT_SECRET=your_jwt_secret
```

---

## 🔐 API Routes Overview

| Route              | Method | Description               |
|-------------------|--------|---------------------------|
| /api/contacts      | GET    | Get all contacts          |
| /api/contacts/:id  | GET    | Get contact by ID         |
| /api/contacts      | POST   | Create new contact        |
| /api/contacts/:id  | PUT    | Update contact            |
| /api/contacts/:id  | DELETE | Delete contact            |
| /api/auth/login    | POST   | Login                     |
| /api/auth/register | POST   | Register new user         |

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).

---

## 🙋‍♂️ Author

**Pawan Varanasi**  
[GitHub: pv1823](https://github.com/pv1823)
