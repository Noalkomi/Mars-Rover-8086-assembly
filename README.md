🚀 Mars Rover Navigation System

A DOS Assembly program that simulates navigating a rover across an 8×8 Martian grid, where hidden craters act as obstacles.

🛠️ Setup Phase
Prompts the user to enter two 8-digit student IDs
Uses the digits to algorithmically generate 6 crater positions
Places the rover (R) at the first available crater-free cell starting from the top-left corner

🎮 Gameplay
Displays an 8×8 grid with a fixed battery limit of 20 units
The player inputs a sequence of moves (U, D, L, R) — up to 20 steps
Moves are executed one at a time, with the screen refreshing after each step

⚠️ Possible Outcomes
Boundary Breach
The rover attempts to leave the grid → error message is displayed and the program terminates
Collision
The rover hits a crater (O) → the cell changes to X, a beep is triggered, and crash coordinates are shown before exiting
Successful Navigation
All moves are executed safely → final coordinates, fuel consumption, and remaining battery are displayed

🔧 Core Procedures
Procedure	Description
obst	Generates crater coordinates from student ID digits
dispgri	Renders the 8×8 grid
showscreen	Refreshes the display after each move
printcoord	Outputs the rover’s current position
printnum	Converts a byte value into decimal for display
