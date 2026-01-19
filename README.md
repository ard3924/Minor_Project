# Food Delivery App

A full-stack food delivery application built with React, Node.js, Express, and MongoDB. It includes a customer-facing frontend, an admin panel for managing the application, and a robust backend API.

## Features

### Customer Frontend

- User registration and login
- Browse food items by category
- Add items to cart
- Place orders with Stripe payment integration
- View order history
- Responsive design

### Admin Panel

- Add new food items
- List and manage food items
- View and manage orders

### Backend API

- User authentication with JWT
- Food item management
- Shopping cart functionality
- Order processing
- Payment processing with Stripe
- Image upload for food items

## Tech Stack

### Frontend & Admin

- React 18
- Vite
- React Router DOM
- Axios for API calls
- React Toastify for notifications
- Stripe.js for payments (frontend only)

### Backend

- Node.js
- Express.js
- MongoDB with Mongoose
- JWT for authentication
- Stripe for payment processing
- Multer for file uploads
- bcrypt for password hashing
- CORS for cross-origin requests

## Prerequisites

- Node.js (latest LTS version)
- MongoDB Atlas account (or local MongoDB)
- Stripe account for payment processing

## Installation and Setup

### 1. Install Node.js

If not already installed, download and install Node.js from [https://nodejs.org/en/download/](https://nodejs.org/en/download/).

### 2. Clone or Download the Project

Open the project folder in VS Code.

### 3. Setup Backend

1. Navigate to the `backend` folder in the terminal.
2. Run `npm install` to install dependencies.
3. Setup MongoDB:
   - Create a MongoDB Atlas account at [https://www.mongodb.com/atlas](https://www.mongodb.com/atlas).
   - Create a new project and database.
   - Set up a database user (avoid '@' in password).
   - Whitelist IP address (0.0.0.0 for all).
   - Get the connection string and replace the placeholder in `backend/config/db.js`.
4. Setup Stripe:
   - Create a Stripe account at [https://stripe.com](https://stripe.com).
   - Get your secret key and add it to a `.env` file in the backend folder:
     ```
     STRIPE_SECRET_KEY=your_stripe_secret_key_here
     ```
5. Run the backend: `npm run server`

### 4. Setup Frontend

1. Navigate to the `frontend` folder in the terminal.
2. Run `npm install` to install dependencies.
3. Run the frontend: `npm run dev`

### 5. Setup Admin Panel

1. Navigate to the `admin` folder in the terminal.
2. Run `npm install` to install dependencies.
3. Run the admin panel: `npm run dev`

## How to Run

1. Start the backend server first: In `backend` folder, run `npm run server`.
2. Start the frontend: In `frontend` folder, run `npm run dev`.
3. Start the admin panel: In `admin` folder, run `npm run dev`.

The application will be available at:

- Frontend: http://localhost:5173 (or similar, check terminal)
- Admin: http://localhost:5174 (or similar, check terminal)
- Backend API: http://localhost:4000

## API Endpoints

- `/api/user` - User authentication
- `/api/food` - Food item management
- `/api/cart` - Shopping cart
- `/api/order` - Order management
- `/images` - Static image serving

## Contributing

Feel free to contribute to this project by submitting issues or pull requests.

