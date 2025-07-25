📁 File Sharing App
A modern, full-stack file sharing application built with the MERN stack, featuring real-time notifications, secure authentication, and cloud storage integration.
🚀 Features
Core Features

Secure File Upload & Download - Upload and share files with advanced security
User Authentication - JWT-based authentication system
Guest Access - Allow anonymous users to upload and download files
Real-time Notifications - Socket.IO powered real-time updates
File Preview - Preview files before downloading
User Dashboard - Personalized dashboard for file management
File Sharing - Generate shareable links for files
Responsive Design - Mobile-friendly interface

Authentication & Security

JWT token-based authentication
Protected routes for authenticated users
Secure file storage with AWS S3
User profile management
Logout functionality

🛠️ Tech Stack
Frontend

React.js - UI framework
Redux Toolkit - State management
Tailwind CSS - Styling
Vite - Build tool
Axios - HTTP client

Backend

Node.js - Runtime environment
Express.js - Web framework
MongoDB - Database
JWT - Authentication
Socket.IO - Real-time communication
AWS S3 - File storage
Multer - File upload handling

📋 Prerequisites
Before running this application, make sure you have the following installed:

Node.js (v14 or higher)
npm or yarn
MongoDB
AWS S3 account (for file storage)

🔧 Installation & Setup
1. Clone the repository
bashgit clone <your-repository-url>
cd file-sharing-app
2. Backend Setup
bashcd server
npm install
Create a .env file in the server directory with the following variables:
envPORT=5000
MONGODB_URI=mongodb://localhost:27017/filesharing
JWT_SECRET=your-jwt-secret-key
JWT_EXPIRY=7d

# AWS S3 Configuration
AWS_ACCESS_KEY_ID=your-aws-access-key
AWS_SECRET_ACCESS_KEY=your-aws-secret-key
AWS_REGION=your-aws-region
AWS_S3_BUCKET_NAME=your-s3-bucket-name

# Other configurations
CLIENT_URL=http://localhost:3000
3. Frontend Setup
bashcd ../client
npm install
4. Start the Application
Start Backend Server
bashcd server
npm start
The server will run on http://localhost:5000
Start Frontend Development Server
bashcd client
npm run dev
The client will run on http://localhost:3000
📁 Project Structure
file-sharing-app/
├── client/                     # Frontend React application
│   ├── public/                 # Public assets
│   ├── src/
│   │   ├── assets/            # Images, logos, screenshots
│   │   ├── components/        # React components
│   │   │   ├── Auth/          # Authentication components
│   │   │   ├── Dashboard/     # Dashboard components
│   │   │   ├── Guest/         # Guest user components
│   │   │   └── ...
│   │   ├── config/            # Configuration files
│   │   ├── redux/             # State management
│   │   │   └── slice/         # Redux slices
│   │   └── ...
│   ├── package.json
│   └── ...
└── server/                     # Backend Node.js application
    ├── src/
    │   ├── config/            # Configuration files
    │   ├── controllers/       # Route controllers
    │   ├── db/               # Database configuration
    │   ├── middlewares/      # Custom middlewares
    │   ├── models/           # Database models
    │   ├── routes/           # API routes
    │   └── ...
    ├── package.json
    └── ...
🔐 API Endpoints
Authentication Routes

POST /api/users/register - User registration
POST /api/users/login - User login
GET /api/users/profile - Get user profile
POST /api/users/logout - User logout

File Routes

POST /api/files/upload - Upload file
GET /api/files - Get user files
GET /api/files/:id - Get specific file
DELETE /api/files/:id - Delete file
GET /api/files/download/:id - Download file

Guest Routes

POST /api/files/guest/upload - Guest file upload
GET /api/files/guest/:id - Guest file access

🎨 Screenshots
The application includes several key screens:

Dashboard - Main user interface
File Upload - Drag and drop file upload
File Preview - Preview files before download
User Profile - Manage user settings
File Sharing - Generate and manage share links

🚀 Deployment
Backend Deployment

Set up environment variables on your hosting platform
Configure MongoDB connection string
Set up AWS S3 bucket and credentials
Deploy to platforms like Heroku, Railway, or DigitalOcean

Frontend Deployment

Build the production version:
bashcd client
npm run build

Deploy to platforms like Vercel, Netlify, or AWS S3

🤝 Contributing

Fork the repository
Create a feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request





Made with ❤️ using MERN Stack
