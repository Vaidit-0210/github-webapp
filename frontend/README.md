# Frontend - React Application

React frontend application with Vite and Tailwind CSS.

## Tech Stack
- **React 19** - UI library
- **Vite** - Build tool and dev server
- **Tailwind CSS** - Styling
- **React Router** - Routing
- **React Hot Toast** - Notifications
- **React Icons** - Icon library

## Project Structure
```
frontend/
├── src/
│   ├── components/     # Reusable components
│   ├── pages/          # Page components
│   ├── context/        # React context
│   ├── utils/          # Utility functions
│   ├── lib/            # Library functions
│   └── main.jsx        # App entry point
└── index.html
```

## Installation

1. **Navigate to frontend directory**
   ```bash
   cd frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```
   
2. **Environment Variables**
   ```bash
   Create a `.env` file in the `frontend/` directory:
   
   Backend API URL # where Express.js API runs
   VITE_API_BASE_URL=http://localhost:5000
   ```

4. **Start development server**
   ```bash
   npm run dev
   ```

## Available Scripts
- `npm run dev` - Start development server
- `npm run build` - Build for production

## Components
- **Sidebar** - Navigation sidebar with auth-aware links
- **ProfileInfo** - User profile information display
- **LikeProfile** - Interactive like/unlike button
- **Search** - User search functionality
- **Repos** - GitHub repositories display
- **Repo** - Individual repository component
- **SortRepos** - Repository sorting functionality
- **Logout** - Secure logout component
- **Spinner** - Loading indicator

## Pages
- **HomePage** - Landing page
- **LoginPage** - GitHub OAuth login
- **SignUpPage** - User registration
- **ExplorePage** - Discover and explore users
- **LikesPage** - View liked profiles

## Features
- GitHub OAuth authentication
- User profile management
- Like/unlike profiles
- Repository display and sorting
- Responsive design with Tailwind CSS
- Toast notifications
- Protected routes


