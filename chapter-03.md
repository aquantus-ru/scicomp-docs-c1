# CHAPTER 3: Linear Structures & String Logic

Linear data structures organize data sequentially. This chapter covers their implementation, usage, and the logic of text processing.

## 1. Arrays and Contiguous Memory
An **array** is a collection of elements identified by index or key.
- **Memory Layout**: Elements are stored in contiguous memory locations.
- **Access**: O(1) random access using the formula: `Address = Base_Address + (Index * Element_Size)`.
- **Insertion/Deletion**: O(n) in the worst case, as elements must be shifted to maintain contiguity.
- **Static vs. Dynamic**: Static arrays have fixed size; dynamic arrays (like Python lists or C++ Vectors) resize automatically by allocating a larger block and copying elements.

## 2. Linked Lists (Single, Double, Circular)
**Linked lists** consist of nodes where each node contains data and a reference (pointer) to the next node.
- **Singly Linked List**: Traversal in one direction. Good for simple queues/stacks.
- **Doubly Linked List**: Nodes point to both next and previous. Allows bidirectional traversal and O(1) deletion if the node is known.
- **Circular Linked List**: The last node points back to the first. Useful for round-robin scheduling.
- **Comparison with Arrays**: Linked lists allow O(1) insertion/deletion at the ends or known positions but strictly O(n) sequential access. They use non-contiguous memory, potentially causing cache misses.

## 3. String Manipulation and Character Encoding
**Strings** are sequences of characters.
- **Immutability**: In many languages (Java, Python), strings are immutable to ensure thread safety and allow string pooling.
- **Encoding**:
  - **ASCII**: 7-bit encoding for English characters.
  - **Unicode**: A universal standard covering most writing systems.
  - **UTF-8**: A variable-width encoding for Unicode (1 to 4 bytes per character). It is backward compatible with ASCII and efficient for Latin scripts.

## 4. Lexical Sorting and Lexicographical Order
**Lexicographical order** is the generalization of alphabetical order to other sequences.
- Comparison is done element by element from the start.
- "Apple" comes before "Banana".
- "10" comes before "2" in string comparison because '1' < '2'.
Sorting algorithms for strings often involve specialized structures like Tries or Radix sort to handle the variable length and character set size efficiently.
