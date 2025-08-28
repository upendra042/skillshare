🌐 Skill Sharing Platform

This project is a Skill Sharing Platform built using Node.js, Express.js, Firebase Firestore, EJS templates, and Sessions.
It provides user roles (User, Tutor, Admin) with features like Login, Signup, Profile Management, Dashboards, Chatbot, Notifications, and more.

🚀 Features

🔑 Authentication & Authorization

Signup and Login with password encryption (bcrypt).

Session-based authentication.

👨‍💻 User Portal

Interactive Chatbot

YouTube Video Generator

Code Generator

Language Converter

Live Chat

Personalized Learning Paths

Community Forum

Profile & Notifications

📊 Tutor Dashboard

Manage skills, bookings, and learning sessions.

🛠 Admin Panel

Manage users, tutors, skills, and analytics.

📖 Blog & Landing Page

🏗 Project Structure
project/
│── views/                # EJS templates (login, signup, dashboards, portal, etc.)
│── public/               # Static files (CSS, JS, images)
│── server.js             # Main Express server file
│── package.json          # Dependencies & project info
│── .env                  # Environment variables
│── README.md             # Project documentation

⚙️ Tech Stack

Backend: Node.js, Express.js

Database: Firebase Firestore

Authentication: bcrypt + express-session

Templating: EJS

Deployment Ready: Configurable with .env

🔧 Setup & Installation
1️⃣ Clone the repository
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name

2️⃣ Install dependencies
npm install

3️⃣ Configure Firebase

Go to Firebase Console

Create a new project

Download service account key JSON

Add it inside your project (replace in server.js)

4️⃣ Environment Variables

Create a .env file in the root:

PORT=3002
SESSION_SECRET=your-secret-key

5️⃣ Run the project
node server.js


Visit 👉 http://localhost:3002

📌 Workflows

User Authentication

Users can sign up with details (name, email, password, etc.).

Passwords are stored securely with bcrypt.

Login verifies password and creates a session.

Role-Based Dashboards

User → Access user portal & learning features.

Tutor → Manage teaching sessions.

Admin → Access admin panel with full control.

Session Management

express-session maintains logged-in state.

Auto redirects users to login if session is missing.

Notifications

Each user has notifications stored in Firestore.

Notifications are shown in the portal.
