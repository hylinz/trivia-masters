# Multiplayer Trivia Game - User Stories with Technologies

## 1. User Management
### Goal: Create basic user functionality and authentication.

- [ ] **User Registration**
  - As a user, I want to register an account so that I can participate in the game.
  - **Technologies**: 
    - Backend: ASP.NET Core MVC (C#), Entity Framework Core (SQL Server)
    - Frontend: React (Forms, Axios for API calls)
  - **Tasks**:
    - Create a database table for users.
    - Build API endpoints for registration.
    - Develop a React form for user input.

- [ ] **User Login**
  - As a user, I want to log into my account so that I can access the game.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, Identity for authentication
    - Frontend: React (Forms, Axios)
  - **Tasks**:
    - Implement login API endpoints.
    - Add JWT-based authentication.
    - Create React components for the login form.

- [ ] **User Logout**
  - As a user, I want to log out of my account so that I can secure my session.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React (Session handling)
  - **Tasks**:
    - Create an API endpoint to invalidate tokens.
    - Add logout functionality to React.

---

## 2. Game Lobby
### Goal: Allow users to create or join game rooms.

- [ ] **View Lobby**
  - As a user, I want to view available game rooms so that I can choose one to join.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React (State management, Axios for API)
  - **Tasks**:
    - Develop API to fetch active game rooms.
    - Build a React component to display room details.

- [ ] **Create Game Room**
  - As a user, I want to create a new game room so that I can play with friends.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR for real-time updates
    - Frontend: React
  - **Tasks**:
    - API endpoint to create a room.
    - Broadcast new room data via SignalR.
    - Add a React form to create rooms.

- [ ] **Join Game Room**
  - As a user, I want to join an existing game room so that I can participate in a trivia session.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: React
  - **Tasks**:
    - API to handle room joining.
    - Notify other players in the room via SignalR.
    - Build UI for joining rooms.

---

## 3. Trivia Gameplay
### Goal: Implement the main trivia functionality.

- [ ] **Start Game**
  - As a host, I want to start the game so that players can begin answering questions.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React (Button actions, Axios)
  - **Tasks**:
    - Create API endpoint to initialize a game.
    - Update React UI for the host to start the game.

- [ ] **Display Questions**
  - As a player, I want to see a trivia question with multiple-choice answers so that I can answer it within the time limit.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React
  - **Tasks**:
    - Fetch questions from the database.
    - Build a React component to display questions and a timer.

- [ ] **Answer Question**
  - As a player, I want to select an answer so that I can compete for points.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React
  - **Tasks**:
    - API endpoint to submit answers.
    - Update React UI for answer selection.

- [ ] **Update Scores**
  - As a user, I want to see my score after each question so that I know how well I am performing.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: React
  - **Tasks**:
    - Calculate scores in the backend.
    - Broadcast score updates via SignalR.
    - Update React UI to display scores.

---

## 4. Real-Time Updates
### Goal: Ensure smooth real-time interactions.

- [ ] **Live Scoreboard**
  - As a player, I want to see an updated scoreboard in real-time so that I can track the competition.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: React
  - **Tasks**:
    - Implement SignalR hub for score updates.
    - Build a React component for the scoreboard.

- [ ] **Room Status**
  - As a user, I want to see when players join or leave the room in real-time so that I stay informed about the game setup.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, SignalR
    - Frontend: React
  - **Tasks**:
    - Update room status with SignalR events.
    - Reflect player changes in the React UI.

---

## 5. Leaderboards
### Goal: Track and display player rankings.

- [ ] **Game Leaderboard**
  - As a player, I want to see the final rankings at the end of a game so that I know who won.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, Entity Framework Core
    - Frontend: React
  - **Tasks**:
    - API endpoint to retrieve game results.
    - Build React UI for end-of-game rankings.

- [ ] **Global Leaderboard**
  - As a user, I want to view the top players globally so that I can compare my performance.
  - **Technologies**:
    - Backend: ASP.NET Core MVC, Entity Framework Core
    - Frontend: React
  - **Tasks**:
    - Create a database table for storing global scores.
    - API to fetch leaderboard data.
    - Build React UI for global leaderboard.

---

## 6. Admin Panel
### Goal: Enable game management by admins.

- [ ] **Manage Questions**
  - As an admin, I want to add, edit, or delete trivia questions so that I can keep the game content updated.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React
  - **Tasks**:
    - API endpoints for CRUD operations on questions.
    - React UI for admin question management.

- [ ] **View Statistics**
  - As an admin, I want to view player statistics and game data so that I can analyze performance trends.
  - **Technologies**:
    - Backend: ASP.NET Core MVC
    - Frontend: React
  - **Tasks**:
    - Build a statistics API.
    - Develop an admin dashboard in React.

---

## 7. Deployment
### Goal: Deploy the application to be accessible online.

- [ ] **Backend Hosting**
  - As a developer, I want to host the C# backend on Azure so that users can access the API.
  - **Technologies**: Azure App Service, Docker (optional)

- [ ] **Frontend Hosting**
  - As a developer, I want to host the React frontend on Vercel or Netlify so that users can access the game in their browser.
  - **Technologies**: Vercel, Netlify

---
