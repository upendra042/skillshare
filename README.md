# 🌐 Skill Sharing Platform  

This project is a **Skill Sharing Platform** built using **Node.js, Express.js, Firebase Firestore, EJS templates, and Sessions**.  
It provides different user roles (**User, Tutor, Admin**) with features like **Login, Signup, Profile Management, Dashboards, Notifications, and more**.  

---

## 🚀 Features  

- 🔑 **Authentication & Authorization** (bcrypt + express-session)  
- 👨‍💻 **User Portal**: Chatbot, Code Generator, Language Converter, Learning Paths, Forum  
- 📊 **Tutor Dashboard**: Manage skills, bookings, sessions  
- 🛠 **Admin Panel**: Manage users, tutors, skills  
- 📖 **Blog & Landing Page**  
- 🔔 **Notifications**: User-specific updates  

---

## 🏗 Project Structure  

```plaintext
project/
│── views/                # EJS templates
│── public/               # Static files (CSS, JS, images)
│── server.js             # Main Express server
│── package.json          # Dependencies
│── .env                  # Environment variables
│── README.md             # Documentation



⚙️ Tech Stack
Backend     : Node.js, Express.js  
Database    : Firebase Firestore  
Auth        : bcrypt + express-session  
Templating  : EJS  

🔧 Setup & Installation
1️⃣ Clone the repository
git clone https://github.com/upendra042/skillshare.git
cd skillshare

2️⃣ Install dependencies
npm install

3️⃣ Configure Firebase

Go to Firebase Console

Create a new project and Firestore DB

Download service account key JSON

Update server.js with your credentials

4️⃣ Create .env file
PORT=3002
SESSION_SECRET=your-secret-key

5️⃣ Run the project
node server.js


Now open 👉 http://localhost:3002

📌 Workflow
flowchart TD
    A[User Signup/Login] --> B{Firestore Verification}
    B -->|Valid User| C[Session Created]
    B -->|Invalid| D[Error: User not found]
    C --> E[Role Check]
    E -->|User| F[User Portal]
    E -->|Tutor| G[Tutor Dashboard]
    E -->|Admin| H[Admin Panel]
    F --> I[Notifications + Features]
    G --> I
    H --> I
