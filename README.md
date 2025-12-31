# Express Taskscape - Backend API

> ITI Graduation Project - A comprehensive project management and task tracking backend system

Taskscape is a robust backend application built with Express.js and TypeScript that facilitates organization management, project creation, and task tracking. It provides RESTful APIs for the admin dashboard and frontend application to manage teams, projects, sprints, and tasks efficiently.

## 🔗 Live Applications

- **Admin Dashboard**: https://taskscape-admin.vercel.app/
- **Frontend Application**: https://taskscape.vercel.app/
- **API Documentation**: https://documenter.getpostman.com/view/19178013/2s9YRB3XUs

## ✨ Features

- **Organization Management**: Create and manage organizations with role-based access control
- **User Authentication**: Secure JWT-based authentication and authorization
- **User Management**: Admin-driven user registration with automated email notifications
- **Project Management**: Create projects and assign team members with specific roles
- **Sprint Management**: Organize work into sprints for agile project management
- **Task Tracking**: Comprehensive task management with start dates, deadlines, and status tracking
- **Real-time Notifications**: WebSocket-based notifications using Socket.io
- **Email Notifications**: Automated email delivery for new account credentials
- **File Upload**: Cloudinary integration for file and image management

## 🛠️ Tech Stack

- **Runtime**: Node.js 18.13
- **Framework**: Express.js
- **Language**: TypeScript
- **Database**: MongoDB with Mongoose ODM
- **Authentication**: JWT (jsonwebtoken) + bcryptjs
- **Validation**: Joi
- **Real-time**: Socket.io
- **Email**: Nodemailer
- **File Upload**: Multer + Cloudinary
- **CORS**: Enabled for cross-origin requests

## 📋 Prerequisites

- Node.js 18.13 or higher
- MongoDB instance (local or cloud)
- Cloudinary account (for file uploads)
- SMTP server credentials (for email notifications)

## 🚀 Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/taskscape-backend.git
   cd express-taskscape
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Set up environment variables**:
   Create a `.env` file in the root directory with the following variables:
   ```env
   PORT=3000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret_key
   
   # Email Configuration
   EMAIL_HOST=smtp.gmail.com
   EMAIL_PORT=587
   EMAIL_USER=your_email@gmail.com
   EMAIL_PASSWORD=your_email_password
   
   # Cloudinary Configuration
   CLOUDINARY_CLOUD_NAME=your_cloud_name
   CLOUDINARY_API_KEY=your_api_key
   CLOUDINARY_API_SECRET=your_api_secret
   ```

4. **Install nodemon** (for development):
   ```bash
   npm install -g nodemon
   ```

5. **Start the development server**:
   ```bash
   npm run start:dev
   ```

6. **Build for production**:
   ```bash
   npm run build
   npm start
   ```

## 📖 Usage

### Workflow Overview

1. **Organization Setup**: 
   - Access the frontend app (https://taskscape.vercel.app/) to create your organization and register an admin account

2. **Team Management**:
   - Access the admin dashboard (https://taskscape-admin.vercel.app/) to create organization members and scrum masters
   - Newly registered employees receive an email with their username and password

3. **Project Creation**:
   - Create projects within the admin dashboard
   - Assign one scrum master and multiple organization members to each project

4. **Sprint & Task Management**:
   - Scrum masters can create sprints within projects
   - Assign tasks to project members with deadlines and priorities
   - Members can view their tasks and update status
   - Scrum masters receive real-time notifications about task status changes

5. **Collaboration**:
   - Members and scrum masters can log in to view their projects, sprints, and tasks
   - Real-time updates keep everyone synchronized

## 📚 API Documentation

Comprehensive API documentation is available at:
https://documenter.getpostman.com/view/19178013/2s9YRB3XUs

## 🏗️ Project Structure

```
express-taskscape/
├── src/
│   ├── controllers/     # Request handlers
│   ├── models/          # Mongoose models
│   ├── routes/          # API routes
│   ├── middleware/      # Custom middleware
│   ├── utils/           # Utility functions
│   └── config/          # Configuration files
├── dist/                # Compiled TypeScript output
├── index.ts             # Application entry point
└── package.json
```

## 🤝 Contributing

This is an ITI graduation project. For contributions or suggestions, please contact the project team.

## 📝 License

ISC

## 👥 Authors

ITI Final Project Team
