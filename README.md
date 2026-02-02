# Color Collide – Multiplayer Network Game

Color Collide is a real-time multiplayer game built with Python, Pygame, and socket programming.  
It uses a client–server network model where multiple clients connect to a central server to compete in the same game room.

---

## 📡 Networking Model

This project uses a **client–server architecture**:
- The **server** manages the game state, player positions, scores, and timing.
- Each **client** controls one player and sends movement data to the server.
- The server sends updated game state back to all clients.

The game uses:
- **TCP sockets** for reliable communication  
- **Fixed-length headers (10 bytes)** to define message sizes  
- **JSON** to encode game data  
- **Multithreading** to handle multiple players simultaneously  

This ensures synchronized gameplay and prevents data loss.

---

## 🧠 Technologies Used

- Python 3
- Pygame
- Socket programming
- JSON data serialization
- Multithreading

---

## 📁 Project Structure
color-collide/
│
├── client.py
├── server.py
├── header_client.py
├── header_server.py
└── README.md

The number of players is controlled by `TOTAL_PLAYERS` in `server.py`.

---

## 🎮 How to Play

- Use the arrow keys to move your square.
- Collide with another player to score a point.
- The game runs for a fixed round time.
- The player with the highest score wins.

---

## 🌐 Network Scope

This game is designed for:
- Localhost (same computer)
- Local Area Network (LAN)

To play over the internet, the server IP address must be shared with clients.

---

## 🚀 Future Improvements

- Chat system
- Player lobby system
- Better collision detection
- Internet-based multiplayer
- Cleaner code structure
- GUI menus

---

## 👨‍💻 Author

Created as a learning project for computer networking and multiplayer game design using Python sockets.


