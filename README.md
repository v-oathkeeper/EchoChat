
# EchoChat - MERN Real-time Chat Application

## Overview
EchoChat is a full-stack real-time chat application built with:
- **MongoDB** (database)
- **Express.js** (backend server)
- **React.js** (frontend)
- **Node.js** (runtime)
- **Socket.IO** (real-time communication)

## Features
- User authentication (login/signup)
- Real-time messaging
- Online status indicators
- Profile customization
- Responsive design
- Cloudinary image uploads

## Installation

### Prerequisites
- Node.js (v20.x recommended)
- MongoDB Atlas URI or local MongoDB instance
- Cloudinary account (for image storage)

### Setup
1. Clone the repository:
```bash
git clone https://github.com/v-oathkeeper/EchoChat
cd EchoChat
```

2. Install dependencies and build:
```bash
npm run build
```

3. Configure environment variables:
Create `.env` in `/backend` with:
```env
PORT=5000
MONGO_URI=your_mongodb_uri
JWT_SECRET=your_jwt_secret
CLOUDINARY_CLOUD_NAME=your_cloud_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
```

4. Start the application:
```bash
npm start
```

## Project Structure
```
EchoChat/
├── backend/
│   ├── src/
│   │   ├── controllers/    # Route handlers
│   │   ├── models/         # MongoDB schemas
│   │   ├── routes/         # API endpoints
│   │   ├── utils/          # Helper functions
│   │   └── index.js        # Server entry point
│   └── .env                # Environment variables
│
├── frontend/
│   ├── public/             # Static assets
│   ├── src/
│   │   ├── components/     # React components
│   │   ├── context/        # State management
│   │   ├── pages/          # Page components
│   │   ├── socket/         # Socket.IO setup
│   │   └── App.js          # Main component
│   └── dist/               # Production build
│
├── .gitignore
└── package.json            # Root project scripts
```

## Development
For development, run frontend and backend separately:

### Frontend Development
```bash
cd frontend
npm run dev
```

### Backend Development
```bash
cd backend
npm run dev
```

## Deployment
The app is configured for deployment on Render:
1. Connects to MongoDB Atlas
2. Automatically builds frontend
3. Serves frontend from Express
4. Handles Socket.IO connections

## Technologies Used
- **Frontend**: React, Vite, Tailwind CSS, DaisyUI
- **Backend**: Node.js, Express, Mongoose
- **Real-time**: Socket.IO
- **Database**: MongoDB
- **Storage**: Cloudinary
- **Authentication**: JWT

## Author
[v-oathkeeper](https://github.com/v-oathkeeper)
```
