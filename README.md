## Greedy Best-First Search for Autonomous Delivery Robots
This project simulates an autonomous delivery robot using the Greedy Best-First Search (Greedy BFS) algorithm to find the optimal path for delivering groceries to various locations within a city grid. The robot needs to navigate around static obstacles such as buildings and vehicles while delivering packages to multiple customer locations.

## Features
City Grid Representation: A 15x15 grid represents the city environment. The grid contains obstacles like buildings, houses, and parked vehicles, while delivery points are assigned randomly within the grid.
Pathfinding with Greedy BFS: The robot uses the Greedy Best-First Search algorithm for navigation, focusing on getting closer to the goal based on the Euclidean distance heuristic.
Dynamic Environment: After each delivery, the start and goal points update to reflect new delivery locations, and the environment adapts accordingly. The robot recalculates its path as needed.
Visualization: The robot’s path, obstacles, and delivery points are visualized in real-time using Python libraries like matplotlib or pygame.
Multi-Delivery Task: The robot performs 5 sequential deliveries, starting each time from the previous delivery location.
## Project Structure
1. Algorithm Implementation:
The Greedy Best-First Search (Greedy BFS) algorithm is used to guide the robot towards the nearest goal, based solely on proximity (Euclidean distance).
The algorithm is evaluated against alternative pathfinding algorithms such as A*, though the focus of this implementation is on Greedy BFS.
2. Environment Representation:
A 15x15 grid is generated to represent the city. Obstacles (buildings, houses, vehicles) are placed at specific locations, and delivery points are assigned randomly.
The robot starts from a fixed location and moves to the assigned delivery points.
3. Path Execution:
The robot follows the calculated path to deliver the package. After each delivery, the environment dynamically changes, and the robot recalculates the new path for the next delivery point.
4. Graphical Interface:
A simple GUI is created using pygame or matplotlib for real-time visualization of the robot's movements, obstacles, and delivery points.
Technologies Used
Python: The main programming language used for implementation.
Pygame: Used for visualizing the robot's movement and the dynamic environment.
Matplotlib: Used for grid visualization and path plotting.
Tkinter: Can be used to create a simple GUI for user interaction.
Setup and Installation
Clone the Repository:

git clone https://github.com/yourusername/Greedy-BFS-Pathfinding-for-Delivery-Robots.git
Install Dependencies: Install the required Python libraries by running:


pip install -r requirements.txt
Run the Simulation: After installation, run the main script to start the simulation:


python Task1_greedyBFS.py
## Usage
Upon running the simulation, the robot will begin its journey from a fixed starting point and navigate the grid.
The user can observe the robot as it navigates to deliver packages while avoiding obstacles.
The environment dynamically changes after each delivery, and the robot adapts to these changes by recalculating the shortest path using the Greedy BFS algorithm.
## Performance Evaluation
## Path Optimality: 
The robot always moves towards the closest delivery point based on Euclidean distance, although this may not always yield the most optimal path when obstacles are considered.
## Execution Time:
Greedy BFS is computationally efficient in terms of quickly finding a path, but it may not always find the best possible path.
## Adaptability: 
The robot can handle dynamic changes in the environment and recalculates paths as necessary when obstacles or delivery points change.
## Future Enhancements
## Comparison with Other Algorithms:
Further work can be done to compare Greedy BFS with other search algorithms, such as A*, in terms of path optimality and execution time.
## Integration of Moving Obstacles:
Implementing moving vehicles or pedestrians as dynamic obstacles would add complexity to the robot's pathfinding capabilities.
## Multiple Robots:
Expanding the project to include multiple delivery robots that collaborate to deliver packages simultaneously.
