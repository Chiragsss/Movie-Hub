# Movie-Hub
Movies Hub is a fully functional web application built using the MERN (MongoDB, Express, React, Node.js) stack. This app allows users to browse, search, and watch movies. It also includes an admin dashboard to manage content and view analytics.

Features

User Features

Browse movies by categories, genres, and trends.

Search for movies using keywords.

Watch movies directly on the platform.

View movie details, including ratings and reviews.

Admin Features

Upload and manage movies.

View analytics for movie views, likes, and comments.

Manage categories, actors, and genres.

Technologies Used

Frontend: React.js

Backend: Node.js, Express.js

Database: MongoDB

Other:

Material-UI for styling.

JWT for authentication.

Axios for API requests.

Installation

Clone the repository:

   git clone https://github.com/yourusername/movies-hub.git
   cd movies-hub

Install dependencies:

   # For backend
   cd backend
   npm install

   # For frontend
   cd ../frontend
   npm install

Set up environment variables:

Create a .env file in the backend directory.

Add the following variables:

MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
PORT=5000

Start the application:

   # Backend
   cd backend
   npm start

   # Frontend
   cd ../frontend
   npm start

Open your browser and navigate to http://localhost:3000 for the frontend.

Folder Structure

movies-hub/
├── backend/
│   ├── config/        # MongoDB and environment configurations
│   ├── controllers/   # Backend logic for movies, users, etc.
│   ├── models/        # Mongoose schemas
│   ├── routes/        # API endpoints
│   └── server.js      # Entry point for the backend server
├── frontend/
│   ├── src/
│   │   ├── components/ # React components
│   │   ├── pages/      # Pages for the app
│   │   ├── context/    # Context API for global state management
│   │   └── App.js      # Main app component
│   └── public/         # Static assets
└── README.md

API Endpoints

Public Routes

GET /api/movies - Fetch all movies.

GET /api/movies/:id - Fetch movie details.

Admin Routes

POST /api/movies - Add a new movie.

PUT /api/movies/:id - Update movie details.

DELETE /api/movies/:id - Delete a movie.
