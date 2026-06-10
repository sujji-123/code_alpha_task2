# Social Media Platform

A mini full-stack Social Media Platform that allows users to create profiles, share posts, interact through comments, follow other users, and build connections in a social networking environment.

## Features

* User Registration & Login
* User Profiles
* Create, Edit & Delete Posts
* Comment on Posts
* Like Posts
* Follow / Unfollow Users
* User Feed
* JWT Authentication
* Responsive Design

## Tech Stack

### Frontend

* React.js
* Vite
* Tailwind CSS
* Axios
* React Router

### Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT
* bcrypt.js

## Project Structure

```text
social-media-platform/
│
├── frontend/
│   ├── src/
│   ├── public/
│   └── package.json
│
├── backend/
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── middleware/
│   │   └── server.js
│   └── package.json
│
├── .gitignore
├── README.md
└── package.json
```

## Database Collections

### Users

* Name
* Username
* Email
* Password
* Profile Picture
* Bio
* Followers
* Following

### Posts

* User ID
* Content
* Image URL (Optional)
* Likes Count
* Comments Count
* Created Date

### Comments

* User ID
* Post ID
* Comment Text
* Created Date

### Followers

* Follower User ID
* Following User ID

## Installation

### Clone Repository

```bash
git clone <repository-url>
cd social-media-platform
```

### Install Dependencies

```bash
yarn install
```

### Start Frontend

```bash
yarn workspace frontend dev
```

### Start Backend

```bash
yarn workspace backend dev
```

### Run Both Services

```bash
yarn dev
```

## Environment Variables

### Backend (.env)

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_secret_key
```

### Frontend (.env)

```env
VITE_API_URL=http://localhost:5000
```

## API Endpoints

### Authentication

* POST /api/auth/register
* POST /api/auth/login

### Users

* GET /api/users/:id
* PUT /api/users/:id
* POST /api/users/follow/:id
* POST /api/users/unfollow/:id

### Posts

* POST /api/posts
* GET /api/posts
* PUT /api/posts/:id
* DELETE /api/posts/:id
* POST /api/posts/like/:id

### Comments

* POST /api/comments
* GET /api/comments/:postId

## Future Enhancements

* Real-Time Chat
* Story Feature
* Notifications
* Image Uploads
* Video Sharing
* Dark Mode
* Hashtags & Search

## License

This project was developed for educational and learning purposes.
