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
│   ├── db.config.js    
│   ├── auth.config.js   
│   └── ...
│
├── controllers/
│   ├── auth.controller.js  
│   ├── user.controller.js  
│   └── ...
│
├── middleware/
│   ├── authJwt.js        
│   ├── verifySignUp.js    
│   └── ...
│
├── models/
│   ├── index.js          
│   ├── user.model.js    
│   └── ...
│
├── routes/
│   ├── auth.routes.js   
│   ├── user.routes.js   
│   └── ...
│
├── services/
│   ├── auth.service.js  
│   ├── user.service.js   
│   └── ...
│
├── utils/
│   ├── bcrypt.js    
│   └── ...
│
├── node_modules/
├── server.js       
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
