# CHAPTER 8: Non-Linear Data Structures

Non-linear structures represent hierarchical or interconnected data.

## 1. Binary Search Trees (BST)
A **binary tree** where for every node:
- Values in the left subtree are smaller.
- Values in the right subtree are larger.
This property enables average O(log n) search, insert, and delete. In the worst case (skewed tree), it degrades to O(n).

## 2. Tree Balancing (AVL, Red-Black)
Self-balancing trees automatically adjust their structure to maintain logarithmic height.
- **AVL Trees**: Strictly balanced using height differences (balance factors). Faster lookups, slower insertions/deletions due to frequent rotations.
- **Red-Black Trees**: Loosely balanced using node coloring rules. Faster insertions/deletions, slightly slower lookups. Used in many standard libraries (e.g., C++ std::map, Java TreeMap).

## 3. Graphs: Adjacency Lists vs. Matrices
**Graphs** consist of vertices (nodes) and edges (connections).
- **Adjacency Matrix**: A 2D array where cell (i, j) represents an edge.
  - Pros: O(1) edge lookup.
  - Cons: O(V^2) space, inefficient for sparse graphs.
- **Adjacency List**: An array of lists where index i contains a list of vertices connected to i.
  - Pros: O(V + E) space, efficient for sparse graphs.
  - Cons: O(V) edge lookup.

## 4. Heaps and Priority Queues
- **Heap**: A complete binary tree satisfying the heap property (Parent >= Child for Max-Heap). Usually implemented as an array.
- **Priority Queue**: An ADT where elements have priority. "Pop" removes the highest priority element.
- Heaps efficiently implement Priority Queues with O(log n) insertion and extraction.
