# Sunset Challenge

<p align="center">
  <img src="https://i.ibb.co/kch2SVb/sunset-logo.png" alt="Sunset Logo" width="200" />
</p>

> Technical assessment for Sunset mid-level software engineer position. A modern todo list with React frontend and NestJS backend.

## 📋 Overview

The Sunset Challenge is a full-stack todo list application developed as part of a technical assessment. The project showcases modern web development practices and technologies, featuring a React frontend and a NestJS backend.

### 🎯 Key Features

- **User Authentication**: Secure login and registration system
- **Todo List Management**: Create, read, update, and delete lists
- **Task Management**: Add, edit, and complete tasks within lists
- **Color Customization**: Personalize lists with custom colors
- **Real-time Updates**: Instant feedback on changes
- **Responsive Design**: Works seamlessly across all devices

## 🏗️ Architecture

The project is divided into two main components:

- [`sunset-challenge-web`](https://github.com/brunownk/sunset-challenge-web): Modern React frontend with TypeScript
- [`sunset-challenge-api`](https://github.com/brunownk/sunset-challenge-api): Robust NestJS backend with PostgreSQL

### Frontend Stack
- React 18 with TypeScript
- Vite for build tooling
- Tailwind CSS for styling
- React Query for state management
- React Hook Form with Zod validation
- Headless UI, Radix UI, and Ark UI for components

### Backend Stack
- NestJS with TypeScript
- PostgreSQL database
- Prisma ORM
- JWT authentication
- RESTful API design
- Docker support

## 🚀 Getting Started

### Prerequisites

- Node.js (v16 or higher)
- Yarn package manager
- PostgreSQL (for local development)
- Git

### Cloning the Repository

To clone this repository with all submodules:

```bash
git clone --recursive git@github.com:brunownk/sunset-challenge.git
```

If you've already cloned the repository without submodules, you can initialize them with:

```bash
git submodule update --init --recursive
```

### Development Setup

1. **Frontend Setup**
```bash
cd sunset-challenge-web
cp .env.example .env
yarn install
yarn dev
```

2. **Backend Setup**
```bash
cd sunset-challenge-api
cp .env.example .env
yarn install
yarn start:dev
```

The applications will be available at:
- Frontend: http://localhost:5172
- Backend: http://localhost:3000

## 📦 Project Structure

```
sunset-challenge/
├── sunset-challenge-web/    # Frontend application
│   ├── src/
│   │   ├── app/            # Application core
│   │   ├── assets/         # Static assets
│   │   ├── Router/         # Application routes
│   │   └── view/           # Page components
│   └── ...
└── sunset-challenge-api/    # Backend API
    ├── src/
    │   ├── auth/           # Authentication module
    │   ├── lists/          # Lists module
    │   ├── tasks/          # Tasks module
    │   └── prisma/         # Database schema
    └── ...
```

## 🔗 API Documentation

The backend API provides the following endpoints:

### Authentication
- `POST /auth/login` - User login
- `POST /auth/register` - User registration
- `POST /auth/refresh` - Token refresh
- `POST /auth/logout` - User logout

### Lists
- `GET /lists` - Get all lists
- `POST /lists` - Create a new list
- `PUT /lists/:id` - Update a list
- `DELETE /lists/:id` - Delete a list

### Tasks
- `GET /tasks` - Get all tasks
- `POST /tasks` - Create a new task
- `PUT /tasks/:id` - Update a task
- `DELETE /tasks/:id` - Delete a task

## 🌐 Production URLs

- Frontend: [https://sunset-challenge-web.vercel.app](https://sunset-challenge-web.vercel.app)
- Backend: [https://sunset-challenge-api.vercel.app](https://sunset-challenge-api.vercel.app)

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- [Sunset](https://sunset-tires.com) for the opportunity
- All open-source libraries and tools used in this project

## 🔄 Navigation

* [Back to Top](#sunset-challenge)
* [Frontend Documentation](https://github.com/brunownk/sunset-challenge-web)
* [Backend Documentation](https://github.com/brunownk/sunset-challenge-api)