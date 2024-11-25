# Multiplayer Trivia Game - User Stories with Technologies

## 1. User Management
### Goal: Create basic user functionality and authentication.

- [ ] **User Registration**
  - As a user, I want to register an account so that I can participate in the game.
  - **Technologies**: 
    - Backend: ASP.NET Core MVC (C#), Entity Framework Core (SQL Server)
    - Frontend: Next.js (React-based forms, Axios for API calls)
    - Deployment: Docker containers for the backend and frontend, AWS ECS for hosting.
  - **Tasks**:
    - Create a database table for users.
    - Build API endpoints for registration.
    - Develop a Next.js page for the registration form.

- [ ] **User Login**
  - As a user, I want to log into my account so that I can access the game.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, Identity for authentication
    - Frontend: Next.js (React-based forms, Axios)
    - Deployment: Docker containers, AWS ECS.
  - **Tasks**:
    - Implement login API endpoints.
    - Add JWT-based authentication.
    - Create a Next.js page for the login form.

- [ ] **User Logout**
  - As a user, I want to log out of my account so that I can secure my session.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js (Session handling)
  - **Tasks**:
    - Create an API endpoint to invalidate tokens.
    - Add logout functionality to the frontend.

---

## 2. Game Lobby
### Goal: Allow users to create or join game rooms.

- [ ] **View Lobby**
  - As a user, I want to view available game rooms so that I can choose one to join.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js (React state management, Axios for API)
  - **Tasks**:
    - Develop an API to fetch active game rooms.
    - Build a Next.js page to display the list of rooms.

- [ ] **Create Game Room**
  - As a user, I want to create a new game room so that I can play with friends.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR for real-time updates
    - Frontend: Next.js
  - **Tasks**:
    - API endpoint to create a room.
    - Broadcast new room data via SignalR.
    - Add a form on the Next.js frontend to create rooms.

- [ ] **Join Game Room**
  - As a user, I want to join an existing game room so that I can participate in a trivia session.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: Next.js
  - **Tasks**:
    - API to handle room joining.
    - Notify other players in the room via SignalR.
    - Build a UI for joining rooms in Next.js.

---

## 3. Trivia Gameplay
### Goal: Implement the main trivia functionality.

- [ ] **Start Game**
  - As a host, I want to start the game so that players can begin answering questions.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js (Button actions, Axios)
  - **Tasks**:
    - Create an API endpoint to initialize a game.
    - Update the Next.js frontend for the host to start the game.

- [ ] **Display Questions**
  - As a player, I want to see a trivia question with multiple-choice answers so that I can answer it within the time limit.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js
  - **Tasks**:
    - Fetch questions from the database.
    - Build a Next.js component to display questions and a timer.

- [ ] **Answer Question**
  - As a player, I want to select an answer so that I can compete for points.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js
  - **Tasks**:
    - API endpoint to submit answers.
    - Update the Next.js frontend for answer selection.

- [ ] **Update Scores**
  - As a user, I want to see my score after each question so that I know how well I am performing.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: Next.js
  - **Tasks**:
    - Calculate scores in the backend.
    - Broadcast score updates via SignalR.
    - Update the Next.js component to display scores.

---

## 4. Real-Time Updates
### Goal: Ensure smooth real-time interactions.

- [ ] **Live Scoreboard**
  - As a player, I want to see an updated scoreboard in real-time so that I can track the competition.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: Next.js
  - **Tasks**:
    - Implement SignalR hub for score updates.
    - Build a scoreboard component in Next.js.

- [ ] **Room Status**
  - As a user, I want to see when players join or leave the room in real-time so that I stay informed about the game setup.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: Next.js
  - **Tasks**:
    - Update room status with SignalR events.
    - Reflect player changes in the Next.js UI.

---

## 5. Leaderboards
### Goal: Track and display player rankings.

- [ ] **Game Leaderboard**
  - As a player, I want to see the final rankings at the end of a game so that I know who won.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, Entity Framework Core
    - Frontend: Next.js
  - **Tasks**:
    - API endpoint to retrieve game results.
    - Build a leaderboard page in Next.js.

- [ ] **Global Leaderboard**
  - As a user, I want to view the top players globally so that I can compare my performance.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, Entity Framework Core
    - Frontend: Next.js
  - **Tasks**:
    - Create a database table for storing global scores.
    - API to fetch leaderboard data.
    - Build a leaderboard page in Next.js.

---

## 6. Admin Panel
### Goal: Enable game management by admins.

- [ ] **Manage Questions**
  - As an admin, I want to add, edit, or delete trivia questions so that I can keep the game content updated.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js
  - **Tasks**:
    - API endpoints for CRUD operations on questions.
    - Build a question management page in Next.js.

- [ ] **View Statistics**
  - As an admin, I want to view player statistics and game data so that I can analyze performance trends.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: Next.js
  - **Tasks**:
    - Build a statistics API.
    - Develop an admin dashboard in Next.js.

---

## 7. Deployment
### Goal: Deploy the application to be accessible online.

- [ ] **Backend Deployment**
  - As a developer, I want to package the backend in a Docker container and deploy it to AWS ECS so that it is scalable and reliable.
  - **Technologies**: Docker, AWS ECS, AWS RDS (SQL Server).

- [ ] **Frontend Deployment**
  - As a developer, I want to package the Next.js frontend in a Docker container and deploy it to AWS ECS so that it is accessible to users globally.
  - **Technologies**: Docker, AWS ECS, AWS S3/CloudFront (for assets).

---
