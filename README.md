CommunityHub

A full-stack community platform that enables users to create, share, and interact with content through posts, likes, and comments. This project demonstrates end-to-end application development, including authentication, API design, database integration, and cloud deployment.

---

🚀 Live Application

- Frontend (Vercel): https://your-frontend.vercel.app
- Backend API (Render): https://your-api.onrender.com/api
- Health Check: https://your-api.onrender.com/api/health

«Replace the URLs above with your actual deployed links.»

---

📌 Problem & Solution

Problem

Many beginner applications stop at local development and fail to demonstrate real-world deployment, authentication, and system integration.

Solution

CommunityHub is built as a production-ready system:

- Fully deployed backend and frontend
- Secure authentication using JWT
- Persistent data storage with MongoDB
- Clean separation of concerns (frontend vs backend)

---

✨ Core Features

🔐 Authentication

- User registration and login
- JWT-based session management
- Protected routes (frontend + backend)

📝 Posts Management

- Create, read, update, delete (CRUD) posts
- View all posts and individual post details

❤️ Social Interactions

- Like posts
- Comment on posts
- Delete comments

⚙️ System Reliability

- Centralized API service layer
- Error handling and validation
- Health check endpoint for monitoring

---

🛠️ Tech Stack

Frontend

- React (Vite)
- React Router
- Context API (Auth state management)

Backend

- Node.js
- Express.js

Database

- MongoDB Atlas
- Mongoose ODM

Authentication

- JSON Web Tokens (JWT)

Deployment

- Vercel (Frontend)
- Render (Backend)

---

📂 Project Structure
```
community-hub/
│
├── backend/
│   ├── config/        # Environment & configuration
│   ├── middleware/    # Auth & error handling
│   ├── models/        # Mongoose schemas
│   ├── routes/        # API endpoints
│   └── server.js      # Entry point
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── context/
│   │   ├── pages/
│   │   └── services/  # API integration
│   └── index.html
│
└── README.md
```
---

⚙️ Getting Started (Local Development)

Prerequisites

- Node.js (v18 or higher)
- MongoDB Atlas account

---

🔧 Installation

1. Clone Repository

git clone https://github.com/Solfegesam/iyf-s10-week-12-Solfegesam.git
cd iyf-s10-week-12-Solfegesam

---

2. Backend Setup

cd backend
npm install

Create ".env" file:

NODE_ENV=development
PORT=3000

MONGODB_URI=your_mongodb_connection_string

JWT_SECRET=your_secure_secret_key
JWT_EXPIRES_IN=7d

FRONTEND_URL=http://localhost:5173

Run backend:

npm run dev

---

3. Frontend Setup

cd ../frontend
npm install

Create ".env" file:

VITE_API_URL=http://localhost:3000/api

Run frontend:

npm run dev

---

🔗 API Endpoints

Authentication

- "POST /api/auth/register" → Register a new user
- "POST /api/auth/login" → Authenticate user
- "GET /api/auth/me" → Get current authenticated user

Posts

- "GET /api/posts" → Fetch all posts
- "GET /api/posts/:id" → Fetch single post
- "POST /api/posts" → Create post (auth required)
- "PUT /api/posts/:id" → Update post (auth required)
- "DELETE /api/posts/:id" → Delete post (auth required)

Comments

- "GET /api/posts/:id/comments" → Get comments
- "POST /api/posts/:id/comments" → Add comment
- "DELETE /api/posts/:id/comments/:commentId" → Delete comment

---

🧪 Health Check

Endpoint:

GET /api/health

Example Response:

{
  "status": "ok",
  "timestamp": "2026-01-01T00:00:00.000Z",
  "database": "connected"
}

---

🚀 Deployment

Backend (Render)

Configuration:

- Build Command: "npm install"
- Start Command: "npm start"

Environment Variables:

NODE_ENV=production
MONGODB_URI=your_production_db_uri
JWT_SECRET=your_production_secret
FRONTEND_URL=https://your-frontend.vercel.app

---

Frontend (Vercel)

Environment Variable:

VITE_API_URL=https://your-api.onrender.com/api

---

⚠️ Key Engineering Challenges

- Handling CORS across environments
- Managing JWT authentication lifecycle
- Synchronizing frontend with deployed backend
- Environment variable consistency in production

---

📈 Future Improvements

- User profile system
- Image upload support (e.g., Cloudinary)
- Search and filtering
- Pagination and performance optimization
- Notifications system

---

👨‍💻 Author

Samuel Barasa
GitHub: https://github.com/Solfegesam

---

🎯 What This Project Demonstrates

- Full-stack architecture design
- RESTful API development
- Authentication & authorization workflows
- Production deployment pipeline
- Debugging and system integration

---

🏁 Final Note

This project represents a complete transition from development to deployment, showcasing the ability to build and ship a real-world full-stack application.

--- 
