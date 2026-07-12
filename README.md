# Quattro-Shift

![React](https://img.shields.io/badge/React-19-61DAFB?logo=react&logoColor=white)
![Node.js](https://img.shields.io/badge/Node.js-Express-339933?logo=node.js&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-Atlas-47A248?logo=mongodb&logoColor=white)
![License](https://img.shields.io/badge/License-Educational-blue)

Quattro-Shift is a full-stack MERN Stack music streaming web application that enables users to upload, stream, organize, and manage music through a modern and intuitive interface. The platform integrates secure authentication using Clerk and utilizes MongoDB GridFS for efficient storage and streaming of audio files.

---

## Features

- Secure user authentication using Clerk
- Upload and stream audio files
- Store audio files using MongoDB GridFS
- Browse all available songs
- Search songs by title, artist, or album
- Create and manage playlists
- Music player with:
  - Play / Pause
  - Previous / Next
  - Seek Bar
  - Volume Control
- Responsive user interface
- RESTful API built with Express.js

---

## MERN Stack

### Frontend

- React.js
- React Router DOM
- Axios
- React Icons
- CSS

### Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- MongoDB GridFS
- Multer

### Authentication

- Clerk

### Development Tools

- Git & GitHub
- Visual Studio Code
- Postman
- Nodemon
- dotenv

---

## Project Structure

```text
Quattro-Shift/
│
├── frontend/
│   ├── src/
│   ├── public/
│   ├── package.json
│
├── backend/
│   ├── config/
│   ├── middleware/
│   ├── models/
│   ├── routes/
│   ├── server.js
│
└── README.md
```

---

## Installation

### Clone the repository

```bash
git clone https://github.com/your-username/Quattro-Shift.git
```

```bash
cd Quattro-Shift
```

### Install dependencies

#### Frontend

```bash
cd frontend
npm install
```

#### Backend

```bash
cd ../backend
npm install
```

---

## Environment Variables

### Frontend (.env)

```env
VITE_CLERK_PUBLISHABLE_KEY=YOUR_CLERK_PUBLISHABLE_KEY
VITE_API_URL=http://localhost:5000
```

### Backend (.env)

```env
PORT=5000

MONGO_URI=YOUR_MONGODB_CONNECTION_STRING

CLERK_SECRET_KEY=YOUR_CLERK_SECRET_KEY
CLERK_PUBLISHABLE_KEY=YOUR_CLERK_PUBLISHABLE_KEY
```

---

## Running the Project

Start the backend

```bash
cd backend
npm start
```

or

```bash
npm run dev
```

Start the frontend

```bash
cd frontend
npm run dev
```

The application will run at:

```text
http://localhost:5173
```

---

## API Endpoints

### Songs

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/songs` | Get all songs |
| GET | `/api/songs/:id` | Get song details |
| GET | `/api/songs/:songId/audio` | Stream audio |
| POST | `/api/songs` | Add a new song |
| PUT | `/api/songs/:id` | Update song |
| DELETE | `/api/songs/:id` | Delete song |

### Playlists

| Method | Endpoint |
|--------|----------|
| GET | `/api/playlists` |
| POST | `/api/playlists` |
| PUT | `/api/playlists/:id` |
| DELETE | `/api/playlists/:id` |

### Upload

| Method | Endpoint |
|--------|----------|
| POST | `/api/upload` |

---

## Database

MongoDB Atlas is used to store:

- User information
- Song metadata
- Playlist details

Audio files are stored efficiently using MongoDB GridFS, enabling seamless audio streaming without relying on third-party storage services.

---

## System Architecture

```text
React.js Client
        │
        ▼
Express.js REST API
        │
        ▼
Node.js Server
        │
        ▼
Clerk Authentication
        │
        ▼
MongoDB Atlas
        │
        ▼
MongoDB GridFS
```

---

## Team

This project was developed as a collaborative group project by:

- Adil Junaid
- Abhishek C
- Hena Suvarnan
- Arshiya Sulfikkar

---

## Future Enhancements

- Favorites and liked songs
- Recently played songs
- Artist profiles
- Album pages
- Shuffle and repeat
- Lyrics integration
- Dark mode
- Mobile application

---

## License

This project is open for learning and educational purposes.

Feel free to explore, learn from, and contribute to the project.
