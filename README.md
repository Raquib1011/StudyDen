# StudyDen

StudyDen is a full-stack MERN web application that helps students discover, share, and evaluate study spots across Dhaka. Users can explore study-friendly locations, check current crowd and noise levels through community check-ins, leave reviews, and help others find the best environment for studying.

---

## Features

### Study Spot Discovery

* Browse study locations across Dhaka
* View detailed information for each study spot
* Search and explore available locations

### Community Check-ins

* Report current crowd level
* Report noise level
* Help other students choose the best time to visit

### Reviews & Ratings

* Leave reviews for study spots
* Rate study environments
* Read feedback from other students

### User Authentication

* User registration
* Secure login using JWT authentication
* Password hashing with bcrypt

### Leaderboard

* View top contributors
* Encourage community participation

### Responsive Design

* Modern UI built with React and Tailwind CSS
* Responsive layout for desktop and mobile devices

---

## Tech Stack

### Frontend

* React
* Vite
* React Router
* Tailwind CSS v4

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose

### Authentication

* JSON Web Token (JWT)
* bcrypt

### APIs

* Barikoi Places API *

---

## Project Structure

```
StudyDen/
│
├── client/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── server/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── controllers/
│   └── package.json
│
└── README.md
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/<your-username>/StudyDen.git
cd StudyDen
```

### Install dependencies

#### Client

```bash
cd client
npm install
```

#### Server

```bash
cd ../server
npm install
```

### Environment Variables

Create a `.env` file inside the server directory.

```env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

---

## Running the Project

### Backend

```bash
cd server
npm run dev
```

### Frontend

```bash
cd client
npm run dev
```

Open the application in your browser at:

```
http://localhost:5173
```

---

## Future Improvements

* Admin dashboard
* Barikoi API integration for automated location import
* Study spot analytics
* Favorites and bookmarks
* Image uploads
* Notifications
* Advanced filtering and recommendations

---

## Software Quality Assurance (SQA) & API Testing

The project includes an automated SQA testing pipeline to ensure backend endpoint reliability, proper HTTP status codes, payload structures, and latency thresholds.

Running Automated API Tests
Make sure your backend server is running on http://localhost:9120, then execute:

```bash
cd server
npm run test:api
```
Test Suite Coverage

* Server Health Check (GET /api/health): Verifies server response, status 200 OK, and execution time under 500ms.

* Public Home Stats (GET /api/home/stats): Validates JSON response structure and public metrics retrieval.

* Spots Directory (GET /api/spots): Ensures correct spot fetching and payload integrity.

Generating Visual Reports
Executing npm run test:api automatically builds an interactive HTML execution report saved inside server/newman/. Open the .html file in any web browser to view detailed visual test assertions.

---

## Learning Outcomes

This project demonstrates experience with:

* Full-stack MERN development
* REST API development
* JWT authentication
* MongoDB database design
* React component architecture
* Responsive UI development
* State management
* CRUD operations
* Client-server communication
* Automated Software Quality Assurance (SQA) and API testing using Postman & Newman CLI.
* CI-ready CLI test integration and visual reporting.
