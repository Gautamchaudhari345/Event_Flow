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
- PostgreSQL / MySQL (any SQL database)  
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

## Installation

### 1. Clone the repository

```bash
git clone https://github.com/your-username/eventflow.git
cd eventflow
