Here's a comprehensive README.md for your MERN stack Bookstore application:

# Bookstore Management System (MERN Stack)


A full-stack bookstore management system with user authentication and book catalog features, built using modern web technologies.

## 🌟 Features

### Backend (Node.js/Express)
- RESTful API endpoints
- MongoDB database integration
- User authentication system
- Password hashing with bcrypt.js
- Book management CRUD operations
- CORS enabled for cross-origin requests
- Environment configuration with dotenv

### Frontend (React)
- Responsive UI with dark mode support
- React Router for navigation
- Context API for state management
- Protected routes for authenticated users
- Toast notifications system
- Modern UI components with Tailwind CSS
- User registration/login system

## 🚀 Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB (local instance or Atlas URI)
- NPM/Yarn



## 🛠️ Project Structure

```
bookstore/
├── server/                 # Backend
│   ├── config/            # Database configuration
│   ├── controller/        # Business logic
│   ├── model/             # MongoDB schemas
│   ├── route/             # API endpoints
│   └── server.js          # Server entry point
│
├── client/                # Frontend
│   ├── public/            # Static assets
│   ├── src/               
│   │   ├── components/    # Reusable UI components
│   │   ├── context/       # Auth context
│   │   ├── pages/         # Application views
│   │   └── App.jsx        # Root component
│   └── vite.config.js     # Build configuration
```

## 🌐 API Endpoints

### Books
- `GET /book` - Get all books

### Users
- `POST /user/signup` - User registration
- `POST /user/login` - User authentication

**Example Request:**
```http
POST /user/signup
Content-Type: application/json

{
  "fullname": "John Doe",
  "email": "john@example.com",
  "password": "securepassword123"
}
```

## 🔒 Authentication Flow
1. User registers via `/signup` endpoint
2. Password is hashed with bcrypt.js
3. User data stored in MongoDB
4. Login validates credentials against stored hash
5. Authentication state managed via React Context
6. Protected routes require valid authentication

## 🎨 Frontend Components
- **AuthProvider**: Global state management
- **Protected Routes**: Course access requires login
- **Dark Mode**: Toggleable dark theme
- **Responsive UI**: Mobile-first design
- **Dynamic Routing**: React Router implementation



**Technologies Used:**
- React 18
- Express.js
- MongoDB
- Mongoose ODM
- Bcrypt.js
- React Router
- Tailwind CSS
- Vite

