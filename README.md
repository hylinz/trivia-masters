# Multiplayer Trivia Game - User Stories

## 1. User Management
### Goal: Create basic user functionality and authentication.

- **User Registration**
  - As a user, I want to register an account so that I can participate in the game.
    - Input: Username, email, password.
    - Output: Confirmation message and account saved in the database.

- **User Login**
  - As a user, I want to log into my account so that I can access the game.
    - Input: Username/email and password.
    - Output: Access to the lobby if credentials are valid.

- **User Logout**
  - As a user, I want to log out of my account so that I can secure my session.
    - Input: Logout button.
    - Output: Redirected to the login page.

---

## 2. Game Lobby
### Goal: Allow users to create or join game rooms.

- **View Lobby**
  - As a user, I want to view available game rooms so that I can choose one to join.
    - Output: A list of active game rooms with player counts.

- **Create Game Room**
  - As a user, I want to create a new game room so that I can play with friends.
    - Input: Room name and privacy setting (public/private).
    - Output: A new room is created and displayed in the lobby.

- **Join Game Room**
  - As a user, I want to join an existing game room so that I can participate in a trivia session.
    - Input: Room ID or selection from the list.
    - Output: Entered into the room's waiting area.

---

## 3. Trivia Gameplay
### Goal: Implement the main trivia functionality.

- **Start Game**
  - As a host, I want to start the game so that players can begin answering questions.
    - Input: Start button.
    - Output: Countdown before the first question.

- **Display Questions**
  - As a player, I want to see a trivia question with multiple-choice answers so that I can answer it within the time limit.
    - Output: Displayed question and timer.

- **Answer Question**
  - As a player, I want to select an answer so that I can compete for points.
    - Input: Selected option.
    - Output: Immediate confirmation of answer submission.

- **Update Scores**
  - As a user, I want to see my score after each question so that I know how well I am performing.
    - Output: Updated score displayed on the leaderboard.

---

## 4. Real-Time Updates
### Goal: Ensure smooth real-time interactions.

- **Live Scoreboard**
  - As a player, I want to see an updated scoreboard in real-time so that I can track the competition.
    - Output: Leaderboard with current scores.

- **Room Status**
  - As a user, I want to see when players join or leave the room in real-time so that I stay informed about the game setup.
    - Output: Notification in the game room.

---

## 5. Leaderboards
### Goal: Track and display player rankings.

- **Game Leaderboard**
  - As a player, I want to see the final rankings at the end of a game so that I know who won.
    - Output: End-of-game leaderboard.

- **Global Leaderboard**
  - As a user, I want to view the top players globally so that I can compare my performance.
    - Output: Global leaderboard with usernames and scores.

---

## 6. Admin Panel
### Goal: Enable game management by admins.

- **Manage Questions**
  - As an admin, I want to add, edit, or delete trivia questions so that I can keep the game content updated.
    - Input: Question text, answer options, correct answer, category.
    - Output: Updated question bank.

- **View Statistics**
  - As an admin, I want to view player statistics and game data so that I can analyze performance trends.
    - Output: Dashboard with key statistics.

---

## 7. Deployment
### Goal: Deploy the application to be accessible online.

- **Backend Hosting**
  - As a developer, I want to host the C# backend on Azure so that users can access the API.

- **Frontend Hosting**
  - As a developer, I want to host the React frontend on Vercel or Netlify so that users can access the game in their browser.

---

## Future Features
### (Optional enhancements)

- **Private Game Invitations**
  - As a user, I want to invite friends to a private game room so that we can play together.

- **Chat System**
  - As a player, I want to chat with other players in the game room so that I can interact socially.

- **Question Categories**
  - As a player, I want to choose question categories before starting a game so that the trivia matches my interests.

---

## Development Order
1. **User Management** (Login, Registration, Logout).
2. **Game Lobby** (View, Create, and Join Rooms).
3. **Trivia Gameplay** (Start Game, Display Questions, Answering).
4. **Real-Time Updates** (SignalR for live interactions).
5. **Leaderboards** (Game and Global Leaderboards).
6. **Admin Panel** (Manage Questions, View Stats).
7. **Deployment** (Backend and Frontend Hosting).
