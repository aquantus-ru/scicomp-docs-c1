# CHAPTER 6: Algorithmic Analysis (Big O)

Algorithmic analysis provides a theoretical framework for estimating the resources (time and memory) an algorithm needs.

## 1. Time and Space Complexity
- **Time Complexity**: How the runtime of an algorithm grows as the input size (n) increases. It is not measured in seconds but in the number of elementary operations.
- **Space Complexity**: How the amount of working memory required grows with the input size. It includes auxiliary space (for variables, stack frames) but usually excludes the space for the input itself.

## 2. Best-case, Average-case, and Worst-case Scenarios
- **Worst-case (Big O)**: The maximum time an algorithm could take. This is the most critical metric for critical systems.
- **Average-case (Big Theta)**: The expected time over all possible inputs. Harder to calculate but useful for general performance (e.g., Quicksort).
- **Best-case (Big Omega)**: The minimum time required (e.g., sorting an already sorted list).

## 3. Asymptotic Notation
We use asymptotic notation to describe growth rates, ignoring constants and lower-order terms.
- **O(1)**: Constant time. Direct access.
- **O(log n)**: Logarithmic. Binary search.
- **O(n)**: Linear. Iterating through a list.
- **O(n log n)**: Linearithmic. Efficient sorting (Merge Sort).
- **O(n^2)**: Quadratic. Nested loops (Bubble Sort).
- **O(2^n)**: Exponential. Recursive algorithms solving NP problems.
- **O(n!)**: Factorial. Brute-force traveling salesman.

## 4. Scalability and Bottleneck Identification
**Scalability** is the ability of a system to handle growing amounts of work.
- An O(n^2) algorithm is not scalable for large datasets compared to O(n log n).
- **Bottleneck Identification**: Profiling code to find the specific section (often the inner loop or a costly I/O operation) that dominates the execution time. Optimizing the bottleneck yields the highest return on investment.
