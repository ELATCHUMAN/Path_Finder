Path Finder Game
Navigate through a maze and find the optimal path to the goal! This Path Finder Game visually demonstrates a breadth-first search (BFS) algorithm to solve mazes in real time.

Features
Dynamic Maze Traversal: Watch the algorithm in action as it finds the shortest path step by step.
Color-Coded Path:
The maze is displayed in blue.
The path being explored is highlighted in red.
Real-Time Visualization: Each step of the algorithm is displayed with a brief delay for clarity.
How It Works
The algorithm starts at the "O" (Start Position).
It uses Breadth-First Search (BFS) to explore all possible moves systematically.
The goal is to reach the "X" (End Position).
Obstacles are represented by "#", and open spaces are represented by " ".
Tech Stack
Python 3.6+
Curses Library: For the terminal-based maze visualization.
Installation
1. Clone the Repository
bash
Copy code
git clone https://github.com/<your-username>/path-finder-game.git
cd path-finder-game
2. Install Python
Ensure Python 3.6+ is installed on your system. Download it from here.

Running the Game
Run the program directly in your terminal using Python:

bash
Copy code
python path_finder.py
How to Play
Run the Program: Launch the script in your terminal.
Watch the Maze Solver:
The red "X" shows the path being explored by the algorithm.
The goal is to reach the "X" in the maze.
Exit the Program: Press any key once the maze has been solved.
Maze Structure
The maze is a 2D grid represented as a list of lists in Python. Here's an example:

python
Copy code
maze = [
    ["#", "O", "#", "#", "#", "#", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", " ", "#", "#", " ", "#", "#", " ", "#"],
    ["#", " ", "#", " ", " ", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", " ", "#"],
    ["#", " ", "#", " ", "#", " ", "#", "#", "#"],
    ["#", " ", " ", " ", " ", " ", " ", " ", "#"],
    ["#", "#", "#", "#", "#", "#", "#", "X", "#"]
]
Symbols:
"O": Starting position.
"X": Ending position (goal).
"#": Walls (obstacles).
" ": Open spaces.
Customizing the Maze
You can customize the maze by modifying the maze variable in the script:

Ensure there’s one "O" (start) and one "X" (end).
Use "#" for walls and " " for open spaces.
Algorithm
This game uses Breadth-First Search (BFS) to find the shortest path:

Start from the "O" position.
Explore all valid neighboring positions (up, down, left, right).
Avoid revisiting already visited positions or walls.
Stop when the "X" position is reached.
Keyboard Controls
No manual input is required during the game.
Press any key to exit the program after the solution is displayed.
