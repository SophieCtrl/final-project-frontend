# Supplement Tracker React App

## Description

This project is the frontend part of a web application that allows users to manage their supplements, track their health goals, and maintain a profile with their health information. The application includes authentication, user profile management, and supplement tracking features.

Complete project: https://github.com/SophieCtrl/supplement-organizer-app/
Backend Part: https://github.com/SophieCtrl/final-project-backend
Deployed project: https://nutritrack-organizer.netlify.app/

## Table of Contents

- Overview
- Features
- Installation
- Usage
- File Structure
- API Endpoints
- Technologies Used
- Contributing
- License

## Features

- User authentication (login, signup, logout)
- Profile management
- Supplement tracking
- Health goals and symptoms tracking
- Filter and search supplements

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/yourusername/final-project-frontend.git
   cd final-project-frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory and add the following environment variables:

   ```env
   MONGODB_URI=your_mongodb_uri
   TOKEN_SECRET=your_jwt_secret
   PORT=5005
   ```

4. Start the server:
   ```bash
   npm run dev
   ```

## Usage

1. Open your browser and navigate to http://localhost:3000.
2. Sign up for a new account or log in with an existing account.
3. Navigate through the application to manage your supplements, profile, and health information.

## File Structure

├── src
│ ├── components
│ │ ├── BrandForm.jsx
│ │ ├── BrandList.jsx
│ │ ├── IsAnon.jsx
│ │ ├── IsPrivate.jsx
│ │ ├── Navbar.jsx
│ ├── context
│ │ ├── auth.context.jsx
│ ├── pages
│ │ ├── HomePage.jsx
│ │ ├── LoginPage.jsx
│ │ ├── ProfilePage.jsx
│ │ ├── SignUpPage.jsx
│ │ ├── SupplementDetailsPage.jsx
│ │ ├── SupplementListPage.jsx
│ │ ├── UserSupplementPage.jsx
│ ├── App.jsx
│ ├── axiosInstance.js
│ ├── main.jsx
│ ├── index.css
├── public
│ ├── filters.json
├── data
├── .env
├── package.json
├── README.md

## API Endpoints

### Authentication

- POST /auth/signup - Sign up a new user
- POST /auth/login - Log in an existing user
- GET /auth/verify - Verify user authentication

### User Profile

- GET /profile - Get user profile
- PUT /profile - Update user profile

### Supplements

- GET /supplements - Get all supplements
- GET /supplements/:id - Get supplement details
- POST /supplements - Add a new supplement
- PUT /supplements/:id - Update supplement details
- DELETE /supplements/:id - Delete a supplement

## Technologies Used

React
React Router
Axios
Context API
Tailwind CSS

## Contributing

1. Fork the repository.
2. Create a new branch (git checkout -b feature-branch).
3. Make your changes.
4. Commit your changes (git commit -m 'Add some feature').
5. Push to the branch (git push origin feature-branch).
6. Open a pull request.

## License

This project is licensed under the MIT License.
