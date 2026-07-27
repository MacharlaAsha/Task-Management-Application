# 📁 Backend Structure

```
server/
│
├── config/
│   └── db.js                  # MongoDB database connection
│
├── controllers/
│   ├── authController.js      # User registration & login logic
│   └── taskController.js      # Task CRUD operations
│
├── middleware/
│   └── authMiddleware.js      # JWT authentication middleware
│
├── models/
│   ├── User.js                # User schema
│   └── Task.js                # Task schema
│
├── routes/
│   ├── authRoutes.js          # Authentication routes
│   └── taskRoutes.js          # Task management routes
│
├── .env                       # Environment variables
├── package.json               # Backend dependencies & scripts
├── server.js                  # Express server entry point
│
└── README.md                  # Backend documentation
```

---

# ✅ Backend Features

### 🔐 Authentication
- User Registration
- User Login
- JWT (JSON Web Token) Authentication
- Password Encryption using bcryptjs
- Protected API Routes

### 📋 Task Management
- Create a Task
- View All Tasks
- View a Single Task
- Update Existing Tasks
- Delete Tasks

### 🗄️ Database
- MongoDB Database
- Mongoose ODM
- User & Task Collections
- One-to-Many Relationship (User → Tasks)

### 🌐 REST API
- Express.js RESTful APIs
- JSON Request & Response Handling
- Error Handling
- Route Protection

### 🛡️ Security
- Password Hashing
- JWT Token Verification
- Authorization Middleware
- Environment Variable Configuration

### ⚙️ Backend Technologies
- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcryptjs
- dotenv
- CORS

### 📡 API Endpoints

#### Authentication
- **POST** `/api/auth/register` – Register a new user
- **POST** `/api/auth/login` – Login and receive JWT token

#### Tasks
- **GET** `/api/tasks` – Get all tasks
- **GET** `/api/tasks/:id` – Get a task by ID
- **POST** `/api/tasks` – Create a new task
- **PUT** `/api/tasks/:id` – Update an existing task
- **DELETE** `/api/tasks/:id` – Delete a task

### 🚀 Backend Capabilities
- Modular Folder Structure
- MVC Architecture
- RESTful API Design
- JWT-Based Authentication
- CRUD Operations
- MongoDB Integration
- Secure Password Storage
- Environment Variable Support
- Scalable and Maintainable Codebase

---

## ▶️ Run the Backend

### Install Dependencies

```bash
npm install
```

### Configure Environment Variables

Create a `.env` file:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

### Start Development Server

```bash
npm run dev
```

### Backend Server

```
http://localhost:5000
```

---

## 📌 Expected Output

After starting the server, you should see:

```
MongoDB Connected Successfully
🚀 Server running on http://localhost:5000
```

The backend is now ready to communicate with the React frontend.
