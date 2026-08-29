# 1. 🫥 Project Introduction

Welcome to Chat App, a real-time messaging application built for seamless communication between users. The project combines a modern React frontend with a Node.js/Express backend and MongoDB database to deliver a smooth chat experience with authentication, live online status, message tracking, and profile management.

This app is designed to be easy to run locally, extend, and customize for your own use case.

# 2. 📝 Project Overview and Features

Chat App is a full-stack real-time chat platform that allows users to:

- Sign up and log in securely
- Send and receive instant messages in real time
- View online/offline presence for other users
- Search for users in a chat sidebar
- See unread message counts
- Update profile information and profile pictures
- View message history between users

### Key Features

- Secure JWT-based authentication
- Real-time updates using Socket.io
- MongoDB-backed persistence for users and messages
- User search and sidebar navigation
- Unread message tracking
- Cloudinary image uploads for profile media and chat images
- Responsive UI built with React + Tailwind CSS

# 3. ⛏️ Tech Stack, APIs, and Other Resources

### Frontend

- React
- Vite
- Tailwind CSS
- React Router DOM
- Axios
- Socket.IO Client
- React Hot Toast

### Backend

- Node.js
- Express.js
- MongoDB with Mongoose
- Socket.IO
- JWT (JSON Web Tokens)
- bcryptjs for password hashing
- Cloudinary for media uploads
- dotenv for environment configuration

### External Services / APIs

- MongoDB Atlas or local MongoDB instance
- Cloudinary media API
- Socket.IO real-time communication layer

# 4. 🧑‍💻 Getting Started: Setup and Running Instructions

## Prerequisites

Before you begin, make sure you have the following installed:

- Node.js (v18 or newer recommended)
- npm or yarn
- MongoDB running locally or a MongoDB Atlas connection string
- A Cloudinary account for image uploads

## 1) Clone the Repository

```bash
git clone https://github.com/Garimabisht12/chat-app.git
cd chat-app
```

## 2) Install Frontend Dependencies

```bash
cd client
npm install
```

## 3) Install Backend Dependencies

```bash
cd ../server
npm install
```

## 4) Configure Environment Variables

### Backend (.env in /server)

Create a `.env` file inside the `server` folder with the following variables:

```env
MONGODB_URI=your_mongodb_connection_string
PORT=5000
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_API_SECRET=your_cloudinary_api_secret
```

### Frontend (.env in /client)

Create a `.env` file inside the `client` folder:

```env
VITE_BACKEND_URL=http://localhost:5000
```

## 5) Run the App

### Start the backend server

```bash
cd server
npm start
```

### Start the frontend app

```bash
cd client
npm run dev
```

Then open the local URL shown in the terminal (typically `http://localhost:5173`) in your browser.

## 6) Project Structure

```text
chat-app/
├── client/                 # React frontend
│   ├── src/
│   ├── context/
│   ├── public/
│   ├── .env
│   └── package.json
├── server/                 # Express backend + Socket.io
│   ├── controllers/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── lib/
│   ├── .env
│   ├── server.js
│   └── package.json
├── README.md
└── .gitignore
```

# 5. 🤝 How to Contribute and Report Issues

Contributions are welcome! If you want to improve the project, please follow these steps:

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Open a pull request with a clear description

### Contribution Guidelines

- Keep the code clean and readable
- Follow the existing project structure and naming conventions
- Test your changes locally before submitting a PR
- Write helpful commit messages

### Reporting Bugs or Issues

If you find a bug or want to suggest a feature:

- Open an issue in the repository
- Include a clear description of the problem
- Mention steps to reproduce it
- Add screenshots if relevant

# 6. 🔥 Conclusion

Chat App is a practical real-time messaging application that demonstrates how to build a modern, responsive, full-stack chat solution with secure authentication, live communication, and scalable backend architecture.

It is suitable as a starter project, learning resource, or foundation for a production-ready messaging platform.

---

Built with passion for real-time communication and modern web development.
