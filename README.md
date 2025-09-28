# GitHub MERN Stack WebApplication

A full-stack MERN application that integrates with GitHub OAuth for authentication and provides social features for developers to connect, explore profiles, and interact with repositories.

## Tech Stack
- **Frontend:** React 19, Vite, Tailwind CSS
- **Backend:** Express.js 5, MongoDB, Passport.js
- **Database:** MongoDB with Mongoose
- **Authentication:** GitHub OAuth 2.0

## Project Structure
```
github-webapp/
├── backend/          # Express.js API server
├── frontend/         # React application
└── package.json      # Root package.json
```

## Prerequisites
```
Node.js v18+ installed
MongoDB instance (local or MongoDB Atlas)
GitHub OAuth App created
```

## Installation

1. **Clone the Repository**
   ```bash
   git clone <repository-url>
   cd github-webapp
   ```

2. **Install all dependencies**
   ```bash
   npm run install:all
   ```

3. **Set up environment variables**
   ```bash
   - Backend: Create `.env` with MongoDB URI and GitHub OAuth credentials
   - Frontend: Create `.env` with API URL
   ```

4. **Start development servers**
   ```bash
   # Terminal 1: Backend
   cd backend && npm run dev
   
   # Terminal 2: Frontend  
   cd frontend && npm run dev
   ```

## Available Scripts
- `npm run install:all` - Install all dependencies
- `npm run build` - Build entire project


