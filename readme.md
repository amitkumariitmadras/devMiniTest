# Authentication Pages (Login, Signup, Signout)

## Project Overview
This project implements full-stack authentication functionality for our app, including Login, Signup, and Signout pages.

### Technologies Used
- **Frontend**: Flutter
- **Backend**: Node.js with Express.js
- **Database**: Firebase

## Features
- **Login**: Users can log in using their email and password.
- **Signup**: New users can register with their name, email, and password.
- **Signout**: Users can log out securely from the app.

## Project Structure

### 1. Frontend - Flutter
#### Login Page
- **Fields**: Email and password.
- **Form Validation**:
  - Check for valid email format.
  - Ensure password meets minimum length requirements.
- **Error Handling**: Display messages for incorrect credentials.

#### Signup Page
- **Fields**: Name, Email, Password, Confirm Password.
- **Form Validation**:
  - Ensure passwords match.
  - Check password strength (e.g., length, special characters).
- **Success Handling**: Display a message upon successful registration.

#### Signout Functionality
- Accessible from the app's home or profile page.
- Displays a confirmation prompt before signing out.

### 2. Backend - Node.js with Express.js
#### API Endpoints
- `POST /signup` - Registers new users.
- `POST /login` - Authenticates users.
- `POST /signout` - Invalidates user session (if applicable).

#### Middleware
- **Input Validation**: Ensures all fields are correctly formatted.
- **Authentication Checks**: Verifies JWT tokens for protected routes.
- **Password Security**:
  - Hashes passwords before storing in the database.
  - Uses bcrypt for hashing.
- **Session Management**:
  - Implements JWT for user session management.
  - Secures API with HTTPS (if possible).

### 3. Database - Firebase
- **User Authentication**:
  - Stores user credentials securely using Firebase Auth.
  - Sets up authentication rules for secure access.

## Acceptance Criteria
1. Users can register, log in, and log out successfully.
2. Form inputs are validated on both frontend and backend.
3. Passwords are securely hashed and not stored in plain text.
4. User sessions are managed securely using JWT or Firebase Auth.
5. Appropriate error and success messages are displayed for user actions.
6. Code is clean, well-documented, and follows best practices.

## Getting Started

### Prerequisites
- Flutter SDK
- Node.js and npm
- Firebase account and setup

### Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/amitkumariitmadras/devMiniTest.git
