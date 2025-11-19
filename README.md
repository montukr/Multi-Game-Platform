Real‑Time Multi‑Game Platform (MERN + Socket.IO)
A modern, real‑time multiplayer web app with a React frontend, Node/Express backend, MongoDB for persistence, and Socket.IO namespaces for live gameplay and a shared lobby.

Features
Live lobby showing active rooms per game with instant updates.

Multiplayer Tic‑Tac‑Toe and Chess with synchronized turns and restart flow.

Single‑player classics (optional): Snake, Tetris, Flappy Bird, Pac‑Man.

Auth flows: register, login, profile and progress tracking.

Clean REST + WebSocket split: REST for auth/profile; sockets for presence/gameplay.

Tech Stack
Frontend: React 18, Vite, React Router, Axios.

Backend: Node.js (LTS), Express 4, Socket.IO v4.

Database: MongoDB + Mongoose.

State: React hooks; socket‑driven state for lobby and games.

Local Development
Prerequisites
Node.js (LTS) and npm

MongoDB running locally (or a remote MongoDB URI)

Repository Structure
client/ — React SPA (Vite)

server/ — Express API + Socket.IO namespaces

env for local
server-
PORT=5000
MONGO_URI=   #mongodb://localhost:27017/multigame 
JWT_SECRET=   #replace_with_long_random_string  
CORS_ORIGIN= # vite client host ip address for multiplayer
# or http://localhost:5173
client-
VITE_API_URL= # vite client host ip address for multiplayer
# http://localhost:5000
VITE_SOCKET_URL=  # vite client host ip address for multiplayer
# http://localhost:5000

