
# Coding Assignment: Build a Massive Multiplayer Game

## Overview
You will build a simple massive multiplayer game using a client-server architecture. The game will be a real-time multiplayer Snake game where multiple players can connect, control their own snake, and compete to survive the longest.

## Game Description: Multiplayer Snake
The game consists of a grid where each player controls a snake. The objective is to navigate the snake around the grid, eat food to grow longer, and avoid colliding with walls or other snakes. The game ends for a player if their snake collides with a wall or another snake. Players can join and leave the game at any time, with the server keeping track of the current state of the game.

## Requirements

### 1. Server
- Handle connections from multiple clients.
- Manage the game state and ensure that moves are valid.
- Broadcast the game state to all clients after each move.
- Determine when a player has lost and remove their snake from the game.

### 2. Client
- Connect to the server.
- Send player moves (directions) to the server.
- Receive and display the game state from the server.
- Handle basic input validation (e.g., ensuring the player cannot move in the opposite direction instantly).

## Technical Specifications
- Use Java for the server implementation.
- Use sockets for communication between the client and server.
- Use native web components for the client implementation.
- The server should run continuously and be able to handle multiple players simultaneously.
- The client should be a web-based application.

## Detailed Instructions

### Server Implementation
1. Setup the server to listen for connections.
2. Manage multiple client connections using threads.
3. Initialize and manage the game state (grid, snakes, food).
4. Handle moves (directions) from clients and validate them.
5. Broadcast the updated game state to all clients.
6. Handle disconnections and remove the corresponding snake.

### Client Implementation
1. Setup web components using HTML, CSS, and JavaScript.
2. Connect to the server using WebSockets.
3. Receive the initial game state from the server.
4. Handle player input (direction controls) and send moves to the server.
5. Receive and display the updated game state.

## Submission Requirements
- Zip file containing server and client code.
- `README.md` with instructions for running the server and client.
- Code should be well-documented and follow best practices.

## Bonus
- Add a scoreboard to display players' current scores.
- Implement power-ups that appear randomly on the grid.
- Enhance user experience with animations and sound effects.

## Evaluation Criteria
- **Correctness:** The game functions as described.
- **Code Quality:** Clean, well-documented code following best practices.
- **User Experience:** Easy setup and gameplay.
- **Robustness:** Server handles edge cases gracefully.

Good luck and happy coding!
