# CHAPTER 7: Sorting and Searching

Ordering data and finding items are fundamental problems in computer science.

## 1. Comparison Sorts (Bubble, Selection, Insertion)
These algorithms sort by comparing elements.
- **Bubble Sort**: Repeatedly swaps adjacent elements if they are in the wrong order. O(n^2). Simple but inefficient.
- **Selection Sort**: Finds the minimum element and places it at the beginning. O(n^2). Minimizes swaps but not comparisons.
- **Insertion Sort**: Builds the sorted array one item at a time. O(n^2) generally, but O(n) for nearly sorted data. Good for small datasets.

## 2. Divide and Conquer (Merge, Quick, Heap)
- **Merge Sort**: Recursively divides the array into halves, sorts them, and merges them. Stable, O(n log n) always. Uses O(n) auxiliary space.
- **Quick Sort**: Picks a pivot and partitions the array into elements less than and greater than the pivot. O(n log n) average, O(n^2) worst case (rare with good pivot selection). In-place and cache-friendly.
- **Heap Sort**: Builds a max-heap and repeatedly extracts the maximum. O(n log n). In-place but not stable.

## 3. Linear vs. Binary Search
- **Linear Search**: Checks every element sequentially. O(n). Works on unsorted data.
- **Binary Search**: Works on sorted arrays. Compares the target with the middle element and discards half the search space. O(log n). Much faster for large datasets.

## 4. Radix and Counting Sorts
Non-comparison sorts can beat the O(n log n) limit by exploiting the structure of the data (e.g., integers).
- **Counting Sort**: Counts the occurrences of each unique value. O(n + k), where k is the range of inputs.
- **Radix Sort**: Sorts numbers digit by digit (least significant to most significant). O(nk), where k is the number of digits.
