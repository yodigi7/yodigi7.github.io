---
title: "Multiplayer Webgame: Seeker vs. Hider"
date: "2025-01-19"
description: "A multiplayer web game where a seeker and hider compete on a 30x30 grid. The seeker, moving faster, tries to tag the hider while limited to seeing only nearby squares—except every 10 seconds when the full grid is revealed. Built with a Svelte frontend and Python backend using WebSockets for real-time updates."
---

This project is a real-time multiplayer webgame where one player acts as a seeker, and the other is a hider, set on a 30x30 grid. The hider has the advantage of perfect visibility across the grid, while the seeker's vision is limited to a 2-square radius. However, every 10 seconds, the seeker gets a brief moment of complete visibility, revealing the hider's location. The seeker's speed is double that of the hider, making the chase dynamic and intense. The seeker's goal is to tag the hider as quickly as possible by occupying the same square as the hider at the same time.

## Design Choices and Implementation

- **Frontend and Backend:**
  The frontend is built with Svelte for a responsive and lightweight UI, while the backend is powered by Python to handle game logic and manage state. The two are connected via websockets for real-time communication.

- **Game State Management:**
  The entire game state resides on the server to minimize cheating opportunities. The server sends the state updates to the client, which simply renders the game visuals. Moves from the client are submitted for every tick, ensuring server-side authority over gameplay.

- **Move Queueing:**
  The client includes a move queue system, allowing players to plan and cancel moves seamlessly. This queue is kept on the frontend to simplify synchronization. Moves are sent to the server only when the next tick requires them, striking a balance between responsiveness and complexity.

- **Websockets for Communication:**
  Websockets were chosen for their low-latency capabilities, making them ideal for real-time updates like player movement and game state changes. Each tick occurs every 0.5 seconds, maintaining smooth gameplay without overwhelming the system.

This project showcases efficient real-time multiplayer mechanics and an emphasis on server-side state management to ensure fairness.