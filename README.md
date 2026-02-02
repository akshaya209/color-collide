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

