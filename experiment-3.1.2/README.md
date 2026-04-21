# Experiment 3.1.2 – Protected Routes with JWT Verification

## Aim
To implement protected routes using JWT authentication with React Router and Express middleware.

## Setup

### Terminal 1 – Backend
```bash
cd jwt-auth-app/server
npm install
node server.js
# Server runs at http://localhost:3001
```

### Terminal 2 – Frontend
```bash
cd jwt-auth-app/client
npm install
npm start
# App runs at http://localhost:3000
```

## Test Credentials
| Field    | Value       |
|----------|-------------|
| Username | admin       |
| Password | password123 |

## Key Technologies
- React 18 + React Router 6
- Express 4 + jsonwebtoken 9
- Axios 1.6 with request interceptor

## Behavior Notes
- Protected routes require a token in localStorage and validate session/token status with backend verification.
- Invalid or expired tokens are rejected by middleware and users are redirected to login.
