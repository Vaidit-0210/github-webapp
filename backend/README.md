# Backend - Express.js API Server

Express.js API server with GitHub OAuth authentication and MongoDB integration.

## Tech Stack
- **Node.js** - JavaScript runtime
- **Express.js 5** - Web framework
- **MongoDB** - Database with Mongoose
- **Passport.js** - Authentication
- **GitHub OAuth** - Authentication strategy

## Project Structure
```
backend/
├── controllers/     # Route controllers
├── routes/          # API routes
├── models/          # Database models
├── middleware/      # Custom middleware
├── db/             # Database connection
├── passport/       # Passport configuration
└── server.js       # Server entry point
```
## Prerequisites
- Node.js v18+ installed
- MongoDB instance (local or Atlas)
- GitHub OAuth App created (Client ID & Secret)

## Installation

1. **Navigate to backend directory**
   ```bash
   cd backend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Set up environment variables**
   ```bash
   # Create .env file
   PORT=5000
   MONGODB_URI=mongodb+srv://<username>:<password>@cluster0.mongodb.net/dbname
   GITHUB_CLIENT_ID=your_github_client_id   # From GitHub Developer Settings
   GITHUB_CLIENT_SECRET=your_github_client_secret # From GitHub Developer Settings
   GITHUB_API_KEY=your_personal_access_token # For GitHub API requests
   CLIENT_BASE_URL=http://localhost:3000    # Frontend URL
   ```

4. **Start development server**
   ```bash
   npm run dev
   ```

## Available Scripts
- `npm run dev` - Start development server with nodemon
- `npm start` - Start production server

## API Routes

### Authentication (`/api/auth`)
- `GET /api/auth/github` - GitHub OAuth login
- `GET /api/auth/github/callback` - OAuth callback
- `POST /api/auth/logout` - Logout user

### Users (`/api/users`)
- `GET /api/users/profile` - Get user profile
- `POST /api/users/like/:username` - Like a profile
- `GET /api/users/likes` - Get liked profiles
- `GET /api/users/explore` - Explore users

### Middleware
- `isAuthenticated` → Protects routes like `/api/users/profile`
