Mars Rover Navigation System 
Overview: A DOS assembly program that simulates navigating a rover across an 8×8 grid on Mars, with craters as obstacles.

Setup Phase

Prompts for two 8-digit student IDs
Uses digits from those IDs to mathematically generate 6 crater positions on the grid
Places the rover (R) at the first crater-free cell starting from the top-left

Gameplay

Displays the grid with a 20-unit fuel/battery limit
Player enters a sequence of moves (U/D/L/R, up to 20)
Moves execute one by one with a screen refresh each step

Outcomes

Boundary breach — rover tries to leave the 8×8 grid → error message, program ends
Collision — rover hits a crater (O) → cell becomes X, beep sounds, crash coordinates printed, program ends
Success — all moves complete without incident → final coordinates, fuel used, and remaining battery are displayed

Key Procedures
ProcedurePurposeobstDerives crater coordinates from student ID digitsdispgriRenders the 8×8 grid to screenshowscreenRefreshes full display during move executionprintcoordPrints rover's current row/colprintnumConverts a byte value to decimal digits for display
