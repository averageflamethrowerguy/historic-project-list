# historic-project-list
A list of projects that I've worked on. These projects are not all public.
Projects are listed most-recent-first.

## ChungOS (Fall 2022)
This is a simple operating system for CS58 (Operating Systems) following the Yalnix spec, as modified by Professor Sean Smith. It has the following features:
1. Boots, intializing virtual memory and loading an init program
2. Handles switching between processes using traps (such as the clock trap)
3. Handles process sycalls, such as `Fork`, `Exec`, `Wait`, `Exit`
4. Implements communication and synchronization datastructures, such as pipes, locks, and cvars
5. Handles communicating with a user via multiple terminals.
Please ask for access to this repository.

## YAME (Yet Another Maze Escaper)
This is a maze escaper for CS69.13 (Multirobot Systems). Several robots start in unknown initial positions, and must completely explore a maze.
1. Each robot will explore the maze using a wall-following algorithm, and a SLAM mapping approach.
2. When two robots are within line-of-sight of one another, they detect each other with cameras
3. They then initiate a map-merge, where each robot updates the other's map.
4. When a complete map is found, a connected traversal graph is generated with a feature-detection approach
5. Robots can then escape the map using a Djisktra's-algorithm approach.
Repository is here: https://github.com/averageflamethrowerguy/cs69-final-project

