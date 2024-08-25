# MAAZ-KHAN-21BCE2085
Turn-Based Chess-like Game with WebSocket Communication This project is a real-time, turn-based game inspired by chess, developed with a server-client architecture using WebSocket for communication.



## Prerequisites
- **Node.js**: Ensure that Node.js is installed on your system.
- **Web Browser**: Any modern web browser (e.g., Chrome, Firefox, Edge) to run the client.

## Setup Instructions

### 1. Clone the Repository
Clone this repository to your local machine using:

git clone https://github.com/maazkhan101/MAAZ-KHAN-21BCE2085.git
</br>
cd project



<h3>1) Server Setup:</h3>

Navigate to the server directory and install the necessary dependencies:
    cd server
    npm install


Start the Server:

Start the WebSocket server:
   node server.js


The server will run on ws://localhost:8080.


<h3>2) Client Setup</h3>

Navigate to the client directory:
    cd ../client

Open the index.html file in your browser:

Alternatively, you can open index.html directly from your file explorer.


Playing the Game

Player Setup:

The game is played between two players. Each player controls five characters, which can include Pawns, Hero1, and Hero2.
Players take turns to make moves according to the game rules described below.

Game Flow:

On their turn, a player clicks on one of their characters and selects a valid move.
The game state updates in real time, displaying the new positions of the characters.
The game ends when one player eliminates all of the opponent's characters.

Game Rules

Grid: The game is played on a 5x5 grid.

Characters:

Pawn: Moves one block in any direction.
Hero1: Moves two blocks straight in any direction.
Hero2: Moves two blocks diagonally in any direction.
Winning Condition: The game ends when one player eliminates all of the opponent's characters.

WebSocket Communication

The server and client communicate via WebSocket events:

Game Initialization: Sets up the game board and character positions.
Player Move: Sends the player's move command to the server.
Game State Update: Broadcasts the updated game state to both players.
Invalid Move Notification: Alerts the player if their move is invalid.
Game Over Notification: Announces the winner and offers a rematch option.

Future Enhancements

Additional Characters: Implement Hero3 and other unique characters.
AI Opponent: Add a basic AI for single-player mode.
Spectator Mode: Allow other users to watch ongoing games.
Ranking System: Track player performance over multiple games.

Edge Cases Handled

Simultaneous Moves: Prevents multiple clients from making moves simultaneously.
Disconnections: Handles disconnections and reconnections during an ongoing game.
Move Validation: Ensures moves are valid before updating the game state.

Contact
For any questions or issues, please contact maazkhancode@gmail.com
