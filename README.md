# TaskFlow - Modern Task Management Platform

<div align="center">

![TaskFlow Logo](https://github.com/user-attachments/assets/fb93cd98-2df5-491f-8ee8-ee7da840aa8b)



**A powerful, collaborative task management application built for modern teams**

[![Live Demo](https://img.shields.io/badge/Live%20Demo-Visit%20App-blue)](https://taskflow-frontend-production-9467.up.railway.app)
[![Backend Repo](https://img.shields.io/badge/Backend-Laravel-blue)](https://github.com/Kyellog-silog/Taskflow-Backend)
[![Frontend Repo](https://img.shields.io/badge/Frontend-React-green)](https://github.com/Kyellog-silog/Taskflow-Frontend)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

[🚀 Live Demo](https://taskflow-frontend-production-9467.up.railway.app) • [📖 Documentation](#documentation) • [🛠️ Setup Guide](#setup-guide)


</div>

## 🌟 Overview

TaskFlow is a modern, full-stack task management application designed to streamline team collaboration and project organization. Built with React and Laravel, it offers a seamless experience with real-time updates, intuitive drag-and-drop interfaces, and powerful team management capabilities.

### ✨ Key Features

- **🎯 Kanban Board Management**: Intuitive drag-and-drop interface for visual project tracking
- **👥 Team Collaboration**: Invite members, assign roles, and manage permissions
- **🔐 Secure Authentication**: JWT-based authentication with Laravel Sanctum
- **⚡ Real-time Updates**: Live synchronization across all connected clients
- **📱 Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **🎨 Modern UI/UX**: Clean, professional interface built with Tailwind CSS
- **🔒 Data Encryption**: Sensitive data encrypted at rest for security
- **📧 Email Invitations**: Automated team invitation system
- **🛡️ Role-based Access**: Granular permission control for team management

## 🚀 Live Application

**Frontend**: [https://taskflow-frontend-production-9467.up.railway.app](https://taskflow-frontend-production-9467.up.railway.app)

**Backend API**: [https://taskflow-backend-production-1a6a.up.railway.app](https://taskflow-backend-production-1a6a.up.railway.app)

## 🛠️ Technology Stack

### Frontend
- **React 18** with TypeScript
- **React Router Dom** - Client-side routing
- **React Query** - Server state management
- **Tailwind CSS** - Utility-first styling
- **@dnd-kit** - Modern drag-and-drop functionality
- **Radix UI** - Accessible component primitives
- **Lucide React** - Beautiful icons
- **Axios** - HTTP client

### Backend
- **Laravel 12** - Modern PHP framework
- **Laravel Sanctum** - SPA authentication
- **PostgreSQL** - Production database (Supabase)
- **SQLite** - Local development database
- **Laravel Mail** - Email functionality
- **Encrypted Eloquent Casts** - Data security

### Infrastructure
- **Railway** - Cloud deployment platform
- **Supabase** - PostgreSQL database hosting
- **SSL/TLS** - End-to-end encryption
- **GitHub Actions** - CI/CD pipeline

## 📸 Screenshots

<div align="center">

### Dashboard
![Dashboard](https://github.com/user-attachments/assets/a6859942-3a5d-457a-a9f0-afd9bd2fa9d4)

### Board Management
![Board Management Page](https://github.com/user-attachments/assets/0a7c4ab4-8ce7-4267-90f7-170189eeb148)
![Board Management Page 2](https://github.com/user-attachments/assets/c804b406-7322-41d5-843a-7cbdfd21eaf8)
![Board Management Page 3](https://github.com/user-attachments/assets/f4fca294-fcd4-400b-a017-4484e846c416)

### Team Management
![Team Management Page](https://github.com/user-attachments/assets/b66768b5-e1d9-4e99-82a0-db2335a3804b)

### Kanban Board
![Kanban Board](https://github.com/user-attachments/assets/05e2fe3b-9854-4984-9bdc-529425966d5b)
![Kanban Board 2](https://github.com/user-attachments/assets/31b94532-fffc-4252-b95b-ddeec76f1847)

### Task Cards
![Task Cards](https://github.com/user-attachments/assets/bede0335-99ff-4d4d-8543-74e3fa125b3c)

</div>

## 🚀 Quick Start

### Prerequisites
- **Node.js** 18+ and npm
- **PHP** 8.2+ with Composer
- **PostgreSQL** (for production) or SQLite (for development)


## 📂 Project Structure  

This repository is the **meta repo** for TaskFlow.  

- **Frontend (React + Tailwind)** → [Taskflow-Frontend](https://github.com/Kyellog-silog/Taskflow-Frontend)  
- **Backend (Laravel + Sanctum)** → [Taskflow-Backend](https://github.com/Kyellog-silog/Taskflow-Backend)  

---

## 🚀 Live Applications  

- **Frontend**: [https://taskflow-frontend-production-9467.up.railway.app](https://taskflow-frontend-production-9467.up.railway.app)  
- **Backend API**: [https://taskflow-backend-production-1a6a.up.railway.app](https://taskflow-backend-production-1a6a.up.railway.app)  

---

## 🛠️ Setup Guide  

Since the code is split into two repositories, please follow setup instructions in their respective repos:

- **Frontend Setup** → [Taskflow-Frontend README](https://github.com/Kyellog-silog/Taskflow-Frontend#readme)  
- **Backend Setup** → [Taskflow-Backend README](https://github.com/Kyellog-silog/Taskflow-Backend#readme)  

---

### Security Features
- ✅ **Data Encryption**: Sensitive user data encrypted at rest
- ✅ **HTTPS/SSL**: All communications encrypted in transit
- ✅ **CORS Protection**: Cross-origin request security
- ✅ **CSRF Protection**: Cross-site request forgery prevention
- ✅ **SQL Injection Prevention**: Parameterized queries
- ✅ **XSS Protection**: Input sanitization and output escaping

## 🏗️ Architecture

```
┌─────────────────┐    ┌──────────────────┐    ┌─────────────────┐
│   React Frontend│    │   Laravel API    │    │   PostgreSQL    │
│                 │    │                  │    │   Database      │
│  • TypeScript   │◄──►│  • REST API      │◄──►│                 │
│  • Tailwind CSS│    │  • Authentication│    │  • Encrypted    │
│  • React Query │    │  • Business Logic│    │  • SSL/TLS      │
└─────────────────┘    └──────────────────┘    └─────────────────┘
```

## 📖 API Documentation

### Authentication Endpoints
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/logout` - User logout
- `GET /api/auth/user` - Get current user

### Team Management
- `GET /api/teams` - List user teams
- `POST /api/teams` - Create new team
- `PUT /api/teams/{id}` - Update team
- `POST /api/teams/{id}/invite` - Invite team member
- `PUT /api/teams/{id}/members/{userId}/role` - Update member role

### Board & Task Management
- `GET /api/boards` - List user boards
- `POST /api/boards` - Create board
- `GET /api/boards/{id}/tasks` - Get board tasks
- `POST /api/tasks` - Create task
- `PUT /api/tasks/{id}` - Update task
- `DELETE /api/tasks/{id}` - Delete task

## 🚢 Deployment

### Railway Deployment

The application is currently deployed on Railway with automatic deployments:

**Backend Configuration**:
```yaml
# railway.toml
[build]
builder = "NIXPACKS"
buildCommand = "composer install --optimize-autoloader --no-dev && php artisan config:cache"

[deploy]
startCommand = "php artisan serve --host=0.0.0.0 --port=$PORT"
```

**Frontend Configuration**:
```yaml
# railway.toml  
[build]
builder = "NIXPACKS"
buildCommand = "npm run build"

[deploy] 
startCommand = "npm start"
```

### Environment Variables

See `RAILWAY_ENV_PRODUCTION.md` for complete production environment setup.

## 🧪 Testing

### Backend Testing
```bash
cd taskflow-backend
php artisan test
```

### Frontend Testing
```bash
cd taskflow-frontend
npm test
```

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit changes**: `git commit -m 'Add amazing feature'`
4. **Push to branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### Development Guidelines
- Follow PSR-12 coding standards for PHP
- Use TypeScript for all frontend code
- Write tests for new features
- Update documentation as needed


## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📞 Support

- **Documentation**: [Project Wiki](https://github.com/Kyellog-silog/taskflow-backend/wiki)
- **Issues**: [GitHub Issues](https://github.com/Kyellog-silog/taskflow-backend/issues)
- **Live Demo**: [TaskFlow App](https://taskflow-frontend-production-9467.up.railway.app)


---

<div align="center">

**[⭐ Star this project](https://github.com/Kyellog-silog/taskflow-backend)** if you find it helpful!

</div>
