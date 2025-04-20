# EventFlow

**EventFlow** is a full-stack event management system built using SQL, Express.js, React.js, JWT for authentication, bcrypt for password hashing, and nodemon for development ease. It supports role-based access for **Organizers** and **Attendees**, allowing users to create, manage, and attend events seamlessly.

## Tech Stack

**Frontend:**  
- React.js  
- Axios  
- Tailwind CSS (optional)

**Backend:**  
- Node.js  
- Express.js  
-  MySQL   
- JWT (JSON Web Tokens)  
- bcrypt.js  
- nodemon (for development)

---

## Features

- User Authentication (Register/Login with JWT)
- Passwords hashed with bcrypt
- Role-based access (Organizer / Attendee)
- Event creation, update, deletion (Organizer only)
- Event listing and registration (Attendee)
- Attendee dashboard with registered events
- Organizer dashboard with created events
- RESTful API architecture

---
## Approach

### Backend (Express.js + SQL)

1. **Project Initialization**:
   - Initialized Node.js project and installed required dependencies like `express`, `bcrypt`, `jsonwebtoken`, `pg` or `mysql2`, `dotenv`, `cors`, and `nodemon`.

2. **Database Setup**:
   - Designed relational schema with tables for `users`, `events`, and `registrations`.
   - Connected Express app to SQL database using a connection pool or ORM.

3. **Authentication**:
   - Implemented registration and login routes.
   - Used `bcrypt` for hashing passwords.
   - Used `JWT` for user authentication and authorization.
   - Created middleware to protect routes based on roles (Organizer or Attendee).

4. **Role-based Access**:
   - Organizers can create, update, delete events.
   - Attendees can view and register for events.

5. **API Structure**:
   - Used RESTful API structure for better scalability.
   - Defined routes like `/api/auth`, `/api/events`, `/api/users`, etc.

---

### Frontend (React.js)

1. **Project Setup**:
   - Used `create-react-app` for scaffolding the frontend.
   - Installed necessary packages like `axios`, `react-router-dom`.

2. **Routing**:
   - Created public and protected routes using `react-router-dom`.
   - Role-based dashboards: Organizer and Attendee have separate views.

3. **Authentication Handling**:
   - Stored JWT token in localStorage after login.
   - Authenticated routes fetch user role and render based on access level.

4. **Event Management**:
   - Organizer can create, edit, delete events via a dashboard.
   - Attendee can view and register for events.

5. **State Management**:
   - Used React hooks and context (or Redux, optional) for managing global auth state and user role.

---

### Final Touches

- Integrated both frontend and backend with CORS enabled.
- Used `nodemon` for live reloading in backend during development.
- Designed clean UI using Tailwind CSS (optional) or basic CSS.




git clone https://github.com/your-username/eventflow.git
cd eventflow
