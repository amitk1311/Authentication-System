🔐 Authentication System API

A secure and scalable authentication & authorization REST API built using Node.js, Express.js, MongoDB, and JWT.
This project demonstrates backend security best practices, including JWT authentication, role-based access control, and password hashing.

🚀 Features

User Signup & Login

JWT-based Authentication (Access Tokens)

Role-Based Access Control (Admin / User)

Secure Password Hashing using bcrypt

Protected Routes using Middleware

Centralized Error Handling

RESTful API Design

MVC Folder Structure

🛠️ Tech Stack

Backend: Node.js, Express.js

Database: MongoDB

Authentication: JWT (JSON Web Token)

Security: bcrypt, middleware-based route protection

Tools: Git, GitHub, Postman

📂 Project Structure
authentication-system-api/
│── controllers/
│   └── authController.js
│── models/
│   └── User.js
│── routes/
│   └── authRoutes.js
│── middleware/
│   ├── authMiddleware.js
│   └── roleMiddleware.js
│── config/
│   └── db.js
│── utils/
│   └── errorHandler.js
│── .env
│── server.js
│── package.json
│── README.md

🔑 API Endpoints
Auth Routes
Method	Endpoint	Description	Access
POST	/api/auth/register	Register new user	Public
POST	/api/auth/login	Login user	Public
GET	/api/auth/profile	Get user profile	Private
GET	/api/auth/admin	Admin-only route	Admin
🔐 Authentication Flow

User registers with email & password

Password is hashed using bcrypt

JWT token is generated on successful login

Token is validated via middleware for protected routes

Role-based middleware restricts admin routes
