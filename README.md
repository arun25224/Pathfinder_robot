# Robot Path Planner

An interactive Python application that visualizes robot pathfinding using the A* search algorithm. The program utilizes the standard turtle graphics library to allow users to draw custom polygonal obstacles on a 2D coordinate plane. Once an obstacle is defined, the system calculates and animates the optimal collision-free path between a predefined start and end point.

## Key Features

* **Interactive Environment:** Users left-click the canvas to plot the vertices of a custom polygon obstacle, and right-click to close the shape and trigger the pathfinding algorithm.
* **A* Pathfinding Algorithm:** Computes the optimal route on a discrete grid by evaluating paths using a Euclidean distance heuristic.
* **Obstacle Inflation:** Automatically expands the user-drawn polygon by a safety margin of 15 units to account for the robot's physical footprint and prevent edge clipping.
* **Collision Detection:** Utilizes counter-clockwise line intersection logic to verify that proposed grid movements do not cross the boundary of the inflated obstacle.

## Prerequisites

The script relies entirely on Python's standard library, requiring no external package installations.
* Python 3.x
* turtle[cite: 10]
* math[cite: 10]

## Usage Instructions

1. Execute the Python script from your terminal or command prompt:
   ```bash
   python "1 obstacle.py"
