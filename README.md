# 🛒 Ecommerce MERN Project

A **full-stack Ecommerce Web Application** built using the **MERN stack** (MongoDB, Express, React, Node.js) with an **Admin Panel** to manage products, orders, and users.


# How to Setup & Run this Project

## 📋 Prerequisites

### Install Node.js (Skip if Already Installed)

1. Visit the official Node.js website: [https://nodejs.org/en/download/](https://nodejs.org/en/download/)
2. Download the Node.js installer for your operating system
3. Run the installer
4. Follow the prompts in the installer to complete installation

---

## 🚀 Project Setup

> **Important:** Run Backend first, then Frontend & Admin

---

## 🔧 Backend Setup

### Step 1: Open Project in VS Code
- Open the backend project folder in Visual Studio Code

### Step 2: Open Integrated Terminal
- Right-click on the sidebar
- Select **"Open In Integrated Terminal"**

### Step 3: Install Dependencies
```bash
npm install
```
Wait for the installation to complete (requires internet connection)

### Step 4: Setup MongoDB Atlas

#### a. Create MongoDB Account
- Visit [MongoDB Atlas](https://www.mongodb.com/cloud/atlas)
- Sign up for a free account

#### b. Create New Project
- Click on **"New Project"** option
- Follow the prompts to create your project

#### c. Build Database
- Navigate to the **Database Section**
- Click **"Build a database"**
- Select **M0 (Free Tier)** and your preferred region
- Click **"Create Database"**

#### d. Create Database User
- Set up a **Username** and **Password**
- Click **"Create User"**
- **Note:** Remember this password for later use

#### e. Configure Network Access
- Add IP address: `0.0.0.0` (allows access from anywhere)
- Click **"Add Entry"**

#### f. Get Connection String
- Click **"Finish & Close"**
- Click **"Connect"**
- Select **"Compass"** option
- Copy the **Connection String**

#### g. Configure Connection in Project
- Open `index.js` in your backend folder
- Paste the connection string
- Replace `<password>` with the password you set in step 4.d
- Save the changes

### Step 5: Run Backend Server
```bash
node .\index.js
```
Your backend server should now be running!

---

## 💻 Frontend & Admin Panel Setup

### Step 1: Open Project in VS Code
- Open the frontend/admin project folder in Visual Studio Code

### Step 2: Open Integrated Terminal
- Right-click on the sidebar
- Select **"Open In Integrated Terminal"**

### Step 3: Install Dependencies
```bash
npm install
```
Wait for the installation to complete (requires internet connection)

### Step 4: Verify Installation
- After installation, you should see a `node_modules` folder in the sidebar

### Step 5: Start the Application
```bash
npm start
```

### Step 6: View in Browser
- The project will automatically open in your default web browser
- If it doesn't open automatically, navigate to `http://localhost:3000`

---

## 📁 Project Structure

```
project-root/
│
├── backend/
│   ├── index.js
│   ├── package.json
│   └── node_modules/
│
├── frontend/
│   ├── src/
│   ├── package.json
│   └── node_modules/
│
└── admin/
    ├── src/
    ├── package.json
    └── node_modules/
```

---

## 🛠️ Technologies Used

- **Frontend:** React.js
- **Backend:** Node.js, Express.js
- **Database:** MongoDB Atlas
- **Package Manager:** npm

---

## ⚠️ Troubleshooting

### Common Issues

**Port Already in Use**
```bash
# Kill the process using the port (Windows)
netstat -ano | findstr :3000
taskkill /PID <PID> /F

# Kill the process using the port (Mac/Linux)
lsof -ti:3000 | xargs kill -9
```

**MongoDB Connection Error**
- Verify your connection string is correct
- Ensure password doesn't contain special characters (or URL encode them)
- Check if IP `0.0.0.0` is added to Network Access

**npm install fails**
- Clear npm cache: `npm cache clean --force`
- Delete `node_modules` and `package-lock.json`
- Run `npm install` again

-



