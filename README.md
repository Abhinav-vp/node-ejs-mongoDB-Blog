# 📝 Blog Application (Node.js + Express + MongoDB)

A full-stack blog application built using **Node.js**, **Express.js**, **MongoDB**, and **EJS**.  
This project demonstrates server-side rendering, RESTful routing, database integration, and a clean MVC-style folder structure.

The application allows users to **create, read, update, and delete (CRUD)** blog posts with a simple and intuitive interface.

---

## 📖 Table of Contents

- Overview  
- Features  
- Tech Stack  
- Project Architecture  
- Folder Structure  
- Installation  
- Environment Variables  
- Running the Application  
- Application Flow  
- Database Schema  
- Common Errors & Fixes  
- Future Enhancements  
- License  
- Author  

---

## 🔍 Overview

This blog application is designed as a learning-friendly yet scalable project.  
It follows best practices such as:
- Separation of concerns  
- Environment-based configuration  
- Modular routing  
- Reusable EJS layouts and partials  

It can be extended easily with authentication, comments, and admin controls.

---

## ✨ Features

- Create blog posts with title and content  
- View all blog posts on the homepage  
- View individual blog posts  
- Edit existing posts  
- Delete posts  
- Server-side rendered views using EJS  
- MongoDB database connection using Mongoose  
- Environment variable support with dotenv  

---

## 🛠 Tech Stack

### Backend
- **Node.js** – JavaScript runtime  
- **Express.js** – Web framework  

### Frontend
- **EJS** – Template engine  
- **HTML5 / CSS3** – Markup and styling  

### Database
- **MongoDB** – NoSQL database  
- **Mongoose** – ODM for MongoDB  

### Tools
- **Nodemon** – Auto-restart server during development  
- **dotenv** – Environment variable management  

---

## 🧱 Project Architecture

The project follows a **MVC-like structure**:

- **Models** → Database schemas  
- **Routes** → Application routes & logic  
- **Views** → UI templates (EJS)  
- **Config** → Database configuration  

---

## 📂 Folder Structure
blog-app/
│
├── app.js # Main application entry point
├── package.json # Project metadata & dependencies
├── package-lock.json
├── .env # Environment variables
│
├── server/
│ ├── config/
│ │ └── db.js # MongoDB connection logic
│ │
│ ├── models/
│ │ └── Blog.js # Blog schema
│ │
│ └── routes/
│ └── blogRoutes.js # Blog routes (CRUD)
│
├── views/
│ ├── layout/
│ │ └── main.ejs # Main layout
│ │
│ ├── partials/
│ │ ├── header.ejs # Navigation bar
│ │ ├── footer.ejs # Footer
│ │ └── search.ejs # Search UI
│ │
│ ├── index.ejs # Homepage
│ ├── create.ejs # Create blog
│ ├── edit.ejs # Edit blog
│ └── view.ejs # Single blog view
│
└── public/
├── css/
│ └── style.css # Stylesheet
└── js/
└── script.js # Client-side JS

---
## Visit
http://localhost:3001
---
## ⚙️ Installation

Setup Database
Sign up for MongoDB free database cluster: MongoDB

### Create .env file
Create a .env file to store your credentials. Example below:

MONGODB_URI=mongodb+srv://<username>:<password>@clusterName.xxxxxxx.mongodb.net/blog
JWT_SECRET=MySecretBlog
### Installation
To install and run this project - install dependencies using npm and then start your server:

$ npm install
$ npm run dev

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/blog-app.git
cd blog-app
---
