
## JWT Authentication Demo

## Overview

This project is a simple Node.js application that demonstrates JWT (JSON Web Token) authentication.
It provides basic user registration, login, and a dashboard feature, along with a front-end HTML form to interact with the authentication system.

![Demo](demo.gif)

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [API Endpoints](#api-endpoints)
- [Front-end](#front-end)

## Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/your-username/JSON-Web-Token-.git
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd jwt-authentication-demo
   ```

3. **Install Dependencies**:

   ```bash
   npm install
   ```

4. **Create a `.env` File**:

   Create a `.env` file in the project root and configure the following environment variables:

   ```dotenv
   PORT=3000
   JWT_SECRET=your-secret-key
   ```

   Replace `your-secret-key` with a strong and secret key for JWT token generation.

## Usage

1. **Start the Server**:

   ```bash
   npm start
   ```

2. **Access the Front-end Form**:

   Open your web browser and go to `http://localhost:3000` to access the front-end form for user authentication.

## Project Structure

The project follows a simple structure:

- `app.js`: The main application file that sets up the Express server and middleware.

- `routes/main.js`: Defines the main API routes for authentication and dashboard.

- `middleware/not-found.js`: Middleware for handling 404 Not Found errors.

- `middleware/error-handler.js`: Middleware for handling errors and returning appropriate responses.

- `controllers/auth.js`: Controller functions for user authentication and token generation.

- `middleware/authentication.js`: Middleware for JWT authentication.

- `public`: Contains static HTML, CSS, and JavaScript files for the front-end.

## API Endpoints

- `/api/v1/register`: Register a user and receive a JWT token in response.

- `/api/v1/login`: Log in with a registered user's credentials and receive a JWT token in response.

- `/api/v1/dashboard`: Access the dashboard data by providing the JWT token in the request headers.

## Front-end

The project includes a basic HTML form for user login and registration in the `public` directory. 
It also has an HTML dashboard page that displays data when authenticated. JavaScript in `browser-app.js` handles form submissions and dashboard interactions.



