# EduHub

EduHub is a comprehensive learning management system (LMS) designed to facilitate connections, teaching, and interaction between tutors and students.

<hr> 

### Deployed Links

<hr> 

### Built With
**Frontend**: React, Tailwind CSS
**Backend**: Node.js, Express, MongoDB, Spring Boot
**SDK**: ZegoCloud for live streaming

<br> <hr>  

### Prerequisites
**Node.js**: v20.11.0
**MongoDB**: Ensure MongoDB is installed and running locally or use a MongoDB Atlas account

<br> <hr> 

### Installation

1. Clone the repository
```bash
git clone https://github.com/DishaAnand/eduhub.git
```

```
cd eduhub
```

2. Backend Setup
- Navigate to the backend directory

```bash
cd backend
```

- Install backend dependencies

```bash
npm install
```

- Set up environment variables

  Create a .env file in the backend directory and add the following:
  ```
  PORT=6002
  MONGO_URI=<Your MongoDB URI>
  JWT_SECRET=<Your JWT Secret>
  ```

- Run the backend server
```bash
npm start
```
The backend will run on http://localhost:6002.

3. Frontend Setup
- Navigate to the frontend directory
```bash
cd ../frontend
```

- Install frontend dependencies

```bash
npm install
```

- Update API URLs

  Modify frontend/src/services/urls.js to point to your local backend:
```javascript
baseURL = 'http://localhost:6002'
```

4. Run the frontend server

```bash
npm start
```

The frontend will run on http://localhost:3000.

<br> <hr> 

### Features

#### User Authentication
- Sign Up: Register new users (Student/Teacher) with encrypted passwords and JWT tokens.
- Login: Authenticate existing users with JWT.
- Forgot Password: Reset password via email link.
- Profile Management: Update user details.
- Logout: Clear user session.

#### Payment Integration
Integrated Stripe for secure payment processing.

#### Community Forum
- Question Posting: Students and tutors can post questions.
- Commenting: Respond to questions and comments.

#### Course Management
- Creation and Editing: Teachers can create and edit courses.
- Viewing: Students can view and enroll in courses.

#### Question Bank and Tests
- Creation: Teachers can create question banks and tests.
- Attempt: Students can attempt tests and view results.

#### Blog Management
Creation, Editing, Listing, and Deletion: Manage blog posts.

#### Dashboard
Course Listing: Display available courses for students to enroll.

<br> <hr> 

### Deployment

- Frontend
  - Vercel: Used for hosting the frontend.
  - Steps: Setting up Vercel account, connecting GitHub repository, configuring build settings, and enabling continuous deployment.
- Backend
  - Render: Used for hosting the backend.
  - Steps: Creating a Render account, deploying backend services, configuring environment variables, and enabling continuous deployment.

<br> <hr> 

### Folder Structure

- Backend
  - constants/: Define application-wide constants.
  - controllers/: Business logic for various features.
  - models/: Mongoose schemas for data structure.
  - routes/: API routes.
  - middlewares/: Pre-validation and request handling.
  - server.js: Entry point of the application.
  - .env: Environment variables (not committed).
  
- Frontend
  - src/assets/: Static resources.
  - src/components/: Reusable UI components.
  - src/pages/: Main pages of the application.
  - tailwind.config.js: Tailwind CSS configuration.
  - postcss.config.js: PostCSS configuration.
  - index.jsx: Entry point of the application.

<br> <hr> 

### License

This project is licensed under the MIT License. See the LICENSE file for details.

<br> <hr> 

### About

EduHub aims to provide an efficient and interactive platform for online learning, helping tutors and students connect seamlessly.

