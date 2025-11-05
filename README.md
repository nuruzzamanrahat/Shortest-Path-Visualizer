# Shortest Path Visualizer (Dijkstra's Algorithm)

This is an interactive web application that finds the shortest path between nodes in a custom-built, weighted, undirected graph. The project visually demonstrates the step-by-step execution of Dijkstra's Algorithm, a key topic of the Optimization Techniques.

This project is built using pure HTML, CSS (with Tailwind CSS for styling), and JavaScript.

## Live Demo & Usage

- **Live Demo**: [► View Live Demo](https://nuruzzamanrahat.github.io/Shortest-Path-Visualizer/)
## Core Concepts

### 1. The Shortest Path Problem

The shortest path problem is a fundamental challenge in graph theory. The goal is to find a path between two vertices (or nodes) in a graph such that the sum of the weights of its constituent edges is minimized.

### 2. Dijkstra's Algorithm

Dijkstra's algorithm is a greedy algorithm used to find the shortest paths from a single source node to all other nodes in a weighted graph.

It works by maintaining a set of unvisited nodes and, for each node, the tentative shortest distance from the source.

The algorithm's main loop:

1. Set the distance to the source node as 0 and all other nodes as Infinity.
2. Select the unvisited node with the smallest tentative distance (this is the "current" node).
3. For the current node, consider all of its unvisited neighbors.
4. Calculate the distance from the source to each neighbor through the current node.
5. If this new path is shorter than the neighbor's previously known distance, update the neighbor's distance.
6. Mark the current node as "visited" (it will not be checked again).
7. Repeat until the destination node is visited or the smallest tentative distance among unvisited nodes is Infinity (meaning no path exists).

## Features

### Interactive Graph Building:

- **Add Nodes**: Click anywhere on the canvas in "Add Node" mode to create a new node (labeled A, B, C...).
- **Add Edges**: Select "Add Edge" mode, click a start node, then an end node. A prompt will ask for a positive integer weight.
- **Delete**: Select "Delete" mode to remove any node or edge with a single click.

### Algorithm Execution:

- Select any node as the "Start" and "End" point from the dropdown menus.
- Click "Find Shortest Path" to run the algorithm.

### Step-by-Step Visualization:

- **Current Node**: The node being processed is highlighted in red.
- **Visited Nodes**: Processed nodes are highlighted in yellow.
- **Final Path**: The final shortest path is highlighted with a thick blue line.

### Detailed Results:

- The "Results" panel shows a log of the algorithm's actions (e.g., "Visiting node C", "Updating distance to D").
- A final "Shortest Path" summary displays the path and the total minimum cost.
- A "Distances from Start" table dynamically updates to show the shortest known distance from the start node to all other nodes as the algorithm runs.

## How to Use the Visualizer

1. **Add Nodes**: Ensure you are in "Add Node" mode (the default). Click on the white canvas area to place nodes.
2. **Add Edges**:
   - Click the "Add Edge" button.
   - Click your first node (it will be highlighted).
   - Click your second node.
   - Enter a weight (e.g., 10) in the pop-up box and press "OK".
3. **Delete (Optional)**: Click the "Delete" button and click on any node or edge to remove it.
4. **Set Path**:
   - Select a "Start" node from the first dropdown.
   - Select an "End" node from the second dropdown.
5. **Run**: Click the "Find Shortest Path" button.
6. **Observe**: Watch the algorithm run step-by-step. The final path and cost will appear in the results panel.
7. **Clear**: Click "Clear Graph" to start over.
