
# RideShare Community App

## Overview
RideShare App is a community-driven ridesharing platform that allows users to connect, share rides, and interact through posts and notifications. The app is structured into two main components: a React Native frontend (`rideshareapp`) for the user interface, and a Node.js backend (`rideshare_backend`) for handling server-side logic and database interactions.

## Key Features
-User Authentication: Secure sign-up and login functionalities.
-Social Features: Ability to follow/unfollow users, create posts, and send messages.
-Notifications: Real-time updates on user interactions.
-Ride Management: Users can schedule, manage, and join rides.
-Dynamic Content: Users can post stories and updates.

## Project Structure
```
RideShareApp/
├── rideshareapp/       # Frontend React Native Application
│   ├── App/
│   │   └── urls.py     # Contains server URL configuration
│   └── ...
└── rideshare_backend/  # Backend Node.js Application
    ├── User.js
    ├── Notification.js
    ├── Post.js
    ├── Rides.js
    ├── Message.js
    ├── Story.js
    └── ...
```

## Installation

### Prerequisites
- Node.js
- React Native environment
- MongoDB

### Setup
1.Clone the repository:
   ```
   cd RideShareApp
   ```

2.Configure the backend:
   - Navigate to the backend folder and install dependencies:
     ```
     cd rideshare_backend
     npm install
     ```
   - Ensure MongoDB is running and accessible.

3.Configure the frontend:
   - Update the `SERVER_URL` in `rideshareapp/App/urls.py` to point to the correct backend server IP and port.
   - Navigate to the frontend folder and install dependencies:
     ```
     cd ../rideshareapp
     npm install
     ```

### Running the Application
1.Start the backend server:
   ```
   cd rideshare_backend
   npm start
   ```

2.Run the frontend application:
   ```
   cd ../rideshareapp
   npm start
   ```

## API Endpoints
Detail some of the core API functionalities available:
-User Authentication: `/api/users/login` and `/api/users/signup`
-Social Interactions: `/api/users/follow` and `/api/users/:id`
-Content Management: `/api/posts/`, `/api/posts/:postId/like`, and `/api/stories`


