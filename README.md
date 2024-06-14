# Node.js Express Login and Registration with JWT Authentication 🚀

## Overview
This project demonstrates a complete user authentication system using Node.js, Express, JWT (JSON Web Tokens), Sequelize (ORM), and MySQL database. It includes user registration, login, and authorization processes.

## Features
- User Registration & Login
- JWT Authentication & Authorization
- Express Middleware for CORS, Authentication & Authorization
- Sequelize ORM for MySQL Database
- Secure Password Hashing
- Error Handling Middleware
- Integration with Front-end Frameworks (Angular, React)

## Project Structure
The project is structured with separation of concerns for better maintainability and scalability:

```
project-root/
│
├── config/
│   ├── db.config.js      # Database configuration
│   ├── auth.config.js    # JWT secret key configuration
│   └── ...
│
├── controllers/
│   ├── auth.controller.js   # Controller for authentication routes
│   ├── user.controller.js   # Controller for user actions
│   └── ...
│
├── middleware/
│   ├── authJwt.js         # JWT authentication middleware
│   ├── verifySignUp.js    # Verify unique username/email middleware
│   └── ...
│
├── models/
│   ├── index.js          # Sequelize initialization and associations
│   ├── user.model.js     # User model definition
│   └── ...
│
├── routes/
│   ├── auth.routes.js    # Routes for authentication (login, register)
│   ├── user.routes.js    # Routes for user actions (profile, etc.)
│   └── ...
│
├── services/
│   ├── auth.service.js   # Authentication service
│   ├── user.service.js   # User service (queries to User model)
│   └── ...
│
├── utils/
│   ├── bcrypt.js         # Password hashing utility
│   └── ...
│
├── node_modules/
├── server.js             # Main server file
├── package.json
└── ...

```

## Getting Started
### Installation
Clone the repository and install dependencies:

```bash
npm install
```

### Configuration
- Configure your MySQL database in `config/db.config.js`.
- Set JWT secret key in `config/auth.config.js`.

### Run
Start the server:

```bash
node server.js
```
