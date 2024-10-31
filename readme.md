# Password Reset 

This project implements a **Password Reset Flow** using `Node.js`, `Express.js`, `Mongoose`, and `React` on the frontend, following the described flow. The backend handles user registration, login, and password reset functionality, while the front-end provides a user-friendly interface built with `React` and styled with `Bootstrap`.

## Task Details

- **Forget Password Page**: The user enters their email address on the forget password page.
- **Check User Existence**: The server checks if the email exists in the database.
  - If the user is not found, an error message is returned.
  - If the user exists, a random string is generated.
- **Send Reset Link**: The random string is stored in the database and emailed to the user as part of a reset link.
- **User Clicks Link**: The user clicks the link, which takes them to a password reset page.
- **Validate Reset Token**: The random string from the link is verified.
  - If valid, the user is shown a form to enter a new password.
  - If the string does not match, an error message is displayed.
- **Password Reset**: After entering the new password, and the password is updated.
  - If the reset is successful, the user can now log in with their new password.

### 2. Technical Specifications

- **Front-End Framework**: React with Bootstrap for UI design.
- **Back-End Framework**: Node.js and Express.js for handling authentication and password reset logic.
- **Database**: MongoDB with Mongoose for data management and user authentication.

## Prerequisites

Make sure you have the following installed:

- **Node.js** (v14+)
- **MongoDB** (local or cloud instance)
- **React** (for front-end)
- **Postman** or **cURL** (for API testing)

# Postman Collection

You can test these API endpoints using Postman. The following link provides a Postman collection that contains all the necessary endpoints for registration, login, forgot password, and password reset functionalities.

[Postman Collection for Password Reset API](https://documenter.getpostman.com/view/39168825/2sAY4vgND2)
