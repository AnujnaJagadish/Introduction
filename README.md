# About me
Uni Student.
To be updated.

# DueDesk

## Project Description

DueDesk is a React-based single-page application (SPA) designed to help students manage their school assignments efficiently. Users can register and log in without passwords, add assignments with due dates, update and mark them as complete, and view their upcoming tasks in an organized and filterable list.

The backend is a Node.js Express server providing RESTful services with full session-based authentication and authorization. The app follows best practices for security, input validation, semantic HTML, and clean React state management.

## How to Use

### Register a User
Go to the registration page and enter a unique username to create your account.  
**Note:** The username `"dog"` is banned and cannot be registered or used.

### Login
Use your registered username to log in. No password is required, but a login step is necessary. Successful login issues a secure session cookie.

### Dashboard
After login, you can:
- Add new assignments with a title and due date.  
- Edit assignments to update titles, due dates, or mark them complete.  
- Filter assignments by completion status and priority.  
- Delete assignments when no longer needed.

### Logout
Log out to clear your session.

### Security & Authorization
- All services except registration and login require a valid session cookie (`sid`).  
- The banned username `"dog"` is explicitly denied permission.  
- User inputs are validated and sanitized on the backend to prevent injection attacks.  
- No passwords are collected or stored.  
- Session IDs are securely generated and stored as `httpOnly` cookies.

## Features

- User registration and login (no passwords required)  
- Assignment CRUD operations (Create, Read, Update, Delete)  
- Mark assignments as done/undone  
- Edit assignment due dates  
- View assignments filtered by completion status  
- Role-based authorization: user "dog" is banned and cannot access protected features  
- Session management using cookies (`sid`) for authentication  
- Frontend input validation and helpful error messages  
- Clean separation of backend routes, data models, and session handling  
- Fully functional using only approved libraries and following all course restrictions

## Getting Started

To run the project locally:

```bash
npm install
npm run build
npm start

- Running `npm run build` to create the static files in the `dist/` directory.
- Running `npm start` to start the Express server.

## Project Structure

- `server.js` — Express server and route handling
- `users.js` — User registration and authentication logic
- `sessions.js` — Session management
- `src/` — React frontend components and styles

## Credits and Licensing

- https://unsplash.com/photos/white-printer-paper-on-white-table-tKSsUjiz5xw
