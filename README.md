# CareerConnect

A full-featured MERN stack job portal inspired by LinkedIn.

## Features
- Candidate, Company, and HR roles
- JWT authentication
- Job CRUD, application status, chat (MongoDB, REST polling)
- File uploads (resume, logo, profile image) via GridFS
- Dashboards for each role
- Responsive UI with Tailwind CSS
- Role-based routing and protected pages

## Tech Stack
- Frontend: React.js, Vite, Tailwind CSS, React Router DOM, Axios, FontAwesome, React Icons
- Backend: Node.js, Express.js, Mongoose, bcryptjs, jsonwebtoken, multer, MongoDB GridFS

## Setup Instructions

### 1. Clone the repository
```
git clone <your-repo-url>
cd CareerConnect
```

### 2. Backend Setup
```
cd server
npm install
cp .env.example .env # Fill in MongoDB URI and JWT secret
npm start
```

### 3. Frontend Setup
```
cd client
npm install
npm run dev
```

### 4. Environment Variables
- See `server/.env.example` for required variables:
  - `MONGO_URI` (MongoDB connection string)
  - `JWT_SECRET` (JWT signing key)
  - `PORT` (default: 5000)
- Frontend uses `VITE_API_URL` in `client/.env` (default: http://localhost:5000)

### 5. File Uploads
- Resume, logo, and profile images are stored in MongoDB using GridFS.

### 6. Running Tests
- Start backend and frontend servers.
- Register users, create jobs, apply, chat, and upload files to validate functionality.

## Folder Structure
- `server/` - Express backend
- `client/` - React frontend

## Deployment
- Use services like Heroku, Vercel, or Render for deployment.
- Set environment variables in production.

## License
MIT
