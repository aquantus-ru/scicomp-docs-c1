# CHAPTER 9: Graph Theory & Traversal

Graph theory models pairwise relations between objects.

## 1. Depth-First Search (DFS)
Traverses as far as possible along each branch before backtracking.
- **Implementation**: Stack (or recursion).
- **Applications**: Topological sorting, detecting cycles, solving mazes.
- **Complexity**: O(V + E).

## 2. Breadth-First Search (BFS)
Explores all neighbor nodes at the present depth before moving to nodes at the next depth level.
- **Implementation**: Queue.
- **Applications**: Finding the shortest path in unweighted graphs, peer-to-peer networks.
- **Complexity**: O(V + E).

## 3. Shortest Path Algorithms (Dijkstra, A*)
- **Dijkstra's Algorithm**: Finds the shortest path from a source to all other nodes in a graph with non-negative weights. Uses a Priority Queue. Greedy approach.
- **A* (A-Star)**: An informed search algorithm used in pathfinding. Uses a heuristic function to estimate the cost to the goal, prioritizing promising paths. Faster than Dijkstra for point-to-point search.

## 4. Spanning Trees and Cycles
- **Minimum Spanning Tree (MST)**: A subset of edges that connects all vertices with the minimum possible total edge weight and no cycles. (Kruskal's and Prim's algorithms).
- **Cycle**: A path that starts and ends at the same vertex. Cycle detection is critical for avoiding infinite loops in dependencies (e.g., build systems).
