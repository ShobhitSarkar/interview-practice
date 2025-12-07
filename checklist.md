# Coding Interview Prep Checklist

## Data Structures

### 1. Arrays
- [ ] Basic array operations (access, insert, delete)
- [ ] Index manipulation
- [ ] In-place modifications
- [ ] Sorting algorithms understanding

#### Problem Solving Patterns
- [ ] Two Pointers
    - [ ] Opposite ends (left/right)
    - [ ] Same direction (fast/slow)
- [ ] Sliding Window
    - [ ] Fixed size window
    - [ ] Variable size window
- [ ] Prefix Sum / Cumulative Sum
- [ ] Kadane's Algorithm (max subarray)
- [ ] Binary Search (on sorted arrays)
- [ ] Cyclic Sort
- [ ] Merge Intervals
- [ ] Partitioning (Dutch National Flag)
- [ ] Fast & Slow Pointers (cycle detection)

---

### 2. Strings
- [ ] String basics (immutability, manipulation)
- [ ] Character operations
- [ ] String comparison

#### Problem Solving Patterns
- [ ] Two Pointers
    - [ ] Palindrome checking
    - [ ] String reversal
- [ ] Sliding Window
    - [ ] Substring problems
    - [ ] Character frequency in window
- [ ] String Matching Algorithms
    - [ ] KMP Algorithm
    - [ ] Rabin-Karp Algorithm
- [ ] Anagram Detection (frequency maps)
- [ ] Subsequence Problems
- [ ] Pattern Matching
- [ ] String Parsing & Tokenization
- [ ] Prefix/Suffix Matching
- [ ] Character Frequency Counting

---

### 3. Hash Tables (HashMap/HashSet)
- [ ] Hash function understanding
- [ ] Collision handling
- [ ] Time complexity (average vs worst case)

#### Problem Solving Patterns
- [ ] Frequency Counting
- [ ] Two Sum Pattern (complement lookup)
- [ ] Group/Categorize Elements
- [ ] Caching & Memoization
- [ ] Detecting Duplicates
- [ ] First Unique Element
- [ ] Mapping Relationships
- [ ] Set Operations (union, intersection, difference)
- [ ] Sliding Window with HashMap
- [ ] Index Mapping

---

### 4. Linked Lists
- [ ] Singly linked list operations
- [ ] Doubly linked list understanding
- [ ] Node manipulation

#### Problem Solving Patterns
- [ ] Fast & Slow Pointers
    - [ ] Cycle detection
    - [ ] Finding middle node
    - [ ] Finding nth from end
- [ ] Reversal
    - [ ] Iterative reversal
    - [ ] Recursive reversal
- [ ] Two Pointers (from different lists)
- [ ] Dummy Node Technique
- [ ] Merging Lists
- [ ] In-place Modifications
- [ ] Runner Technique
- [ ] Partitioning
- [ ] Finding Intersection
- [ ] Removing Nodes

---

### 5. Stacks
- [ ] LIFO principle
- [ ] Push/Pop/Peek operations
- [ ] Stack implementation (array vs linked list)

#### Problem Solving Patterns
- [ ] Monotonic Stack
    - [ ] Next greater element
    - [ ] Next smaller element
- [ ] Parentheses/Bracket Matching
- [ ] Expression Evaluation
    - [ ] Infix to postfix
    - [ ] Postfix evaluation
    - [ ] Prefix evaluation
- [ ] Backtracking with Stack
- [ ] Function Call Simulation
- [ ] Undo Operations
- [ ] Nested Structures
- [ ] Min/Max Stack
- [ ] Stock Span Problems
- [ ] Histogram Problems (largest rectangle)

---

### 6. Queues
- [ ] FIFO principle
- [ ] Enqueue/Dequeue operations
- [ ] Circular queue understanding

#### Problem Solving Patterns
- [ ] BFS Traversal
- [ ] Sliding Window Maximum/Minimum
- [ ] Level Order Processing
- [ ] Deque for Sliding Window
- [ ] Circular Queue
- [ ] Priority Queue Simulation
- [ ] Request Processing
- [ ] Recent Counter Problems
- [ ] Moving Average
- [ ] Stream Processing

---

### 7. Binary Trees
- [ ] Tree terminology (root, leaf, height, depth)
- [ ] Tree traversal basics
- [ ] Tree properties

#### Problem Solving Patterns
- [ ] DFS Traversals
    - [ ] Preorder (Root-Left-Right)
    - [ ] Inorder (Left-Root-Right)
    - [ ] Postorder (Left-Right-Root)
- [ ] BFS/Level Order Traversal
- [ ] Recursive Tree Problems
- [ ] Path Sum Problems
- [ ] Tree Construction (from traversals)
- [ ] Lowest Common Ancestor (LCA)
- [ ] Tree Serialization/Deserialization
- [ ] Diameter/Height Calculations
- [ ] Subtree Problems
- [ ] Morris Traversal (O(1) space)

---

### 8. Binary Search Trees (BST)
- [ ] BST property (left < root < right)
- [ ] BST operations
- [ ] Balanced vs unbalanced trees

#### Problem Solving Patterns
- [ ] Inorder Traversal (sorted output)
- [ ] BST Validation
- [ ] Search/Insert/Delete Operations
- [ ] Kth Smallest/Largest Element
- [ ] Range Queries
- [ ] BST to Sorted Array
- [ ] Two Sum in BST
- [ ] LCA in BST
- [ ] Convert Sorted Array to BST
- [ ] BST Iterator

---

### 9. Heaps (Priority Queue)
- [ ] Min heap vs Max heap
- [ ] Heap operations (insert, extract, peek)
- [ ] Heapify process

#### Problem Solving Patterns
- [ ] Top K Elements
- [ ] K-way Merge
- [ ] Median Maintenance (two heaps)
- [ ] Meeting Rooms Problems
- [ ] Task Scheduling
- [ ] Merge K Sorted Lists/Arrays
- [ ] Kth Largest/Smallest
- [ ] Frequency-based Problems
- [ ] Continuous Median
- [ ] Connection Cost Problems

---

### 10. Graphs
- [ ] Graph representation (adjacency list/matrix)
- [ ] Directed vs undirected graphs
- [ ] Weighted vs unweighted graphs

#### Problem Solving Patterns
- [ ] DFS (Depth-First Search)
    - [ ] Recursive implementation
    - [ ] Iterative implementation
- [ ] BFS (Breadth-First Search)
- [ ] Topological Sort
    - [ ] Kahn's Algorithm
    - [ ] DFS-based approach
- [ ] Cycle Detection
    - [ ] In directed graphs
    - [ ] In undirected graphs
- [ ] Union Find / Disjoint Set
- [ ] Dijkstra's Algorithm (shortest path)
- [ ] Connected Components
- [ ] Bipartite Checking
- [ ] Clone Graph
- [ ] Path Finding Problems

---

### 11. Tries (Prefix Trees)
- [ ] Trie structure and nodes
- [ ] Insert/Search operations
- [ ] Space complexity considerations

#### Problem Solving Patterns
- [ ] Prefix Matching
- [ ] Auto-complete
- [ ] Word Search in Matrix
- [ ] Longest Common Prefix
- [ ] Word Dictionary (add/search with wildcards)
- [ ] Replace Words
- [ ] Stream of Characters
- [ ] Maximum XOR Problems
- [ ] Phone Directory
- [ ] IP Routing (longest prefix match)

---

### 12. Dynamic Programming
- [ ] Memoization (top-down)
- [ ] Tabulation (bottom-up)
- [ ] State definition
- [ ] Recurrence relation

#### Problem Solving Patterns
- [ ] 1D DP (Fibonacci-style)
- [ ] 2D DP (Grid problems)
- [ ] Knapsack Variants
    - [ ] 0/1 Knapsack
    - [ ] Unbounded Knapsack
    - [ ] Bounded Knapsack
- [ ] Longest Common Subsequence (LCS)
- [ ] Longest Increasing Subsequence (LIS)
- [ ] Matrix Chain Multiplication
- [ ] Palindrome Problems
- [ ] Edit Distance
- [ ] Coin Change Problems
- [ ] House Robber Variants
- [ ] Stock Trading Problems
- [ ] State Machine DP
- [ ] DP with Bitmasks
- [ ] Interval DP

---

### 13. Backtracking
- [ ] Backtracking template
- [ ] Decision tree understanding
- [ ] Pruning strategies

#### Problem Solving Patterns
- [ ] Permutations
- [ ] Combinations
- [ ] Subsets (Powerset)
- [ ] N-Queens
- [ ] Sudoku Solver
- [ ] Word Search
- [ ] Generate Parentheses
- [ ] Letter Combinations
- [ ] Palindrome Partitioning
- [ ] Combination Sum Variants

---

### 14. Greedy Algorithms
- [ ] Greedy choice property
- [ ] Optimal substructure
- [ ] Proof of correctness

#### Problem Solving Patterns
- [ ] Activity Selection
- [ ] Interval Scheduling
- [ ] Jump Game
- [ ] Gas Station
- [ ] Minimum Platforms
- [ ] Fractional Knapsack
- [ ] Huffman Encoding
- [ ] Task Assignment
- [ ] Partition Problems
- [ ] Two City Scheduling

---

### 15. Bit Manipulation
- [ ] Bitwise operators (AND, OR, XOR, NOT)
- [ ] Bit shifting (left, right)
- [ ] Common bit tricks

#### Problem Solving Patterns
- [ ] Single Number (XOR tricks)
- [ ] Counting Bits
- [ ] Power of Two
- [ ] Reverse Bits
- [ ] Bitwise AND of Range
- [ ] Subset Generation Using Bits
- [ ] Brian Kernighan's Algorithm
- [ ] Bitmasking for DP
- [ ] Hamming Distance
- [ ] Missing Number

---

### 16. Matrix/2D Arrays
- [ ] Matrix traversal
- [ ] Row-major vs column-major
- [ ] Matrix operations

#### Problem Solving Patterns
- [ ] DFS/BFS on Matrix
- [ ] Spiral Traversal
- [ ] Rotation (90°, 180°)
- [ ] Set Matrix Zeroes
- [ ] Island Problems
- [ ] Word Search
- [ ] Dynamic Programming on Grid
- [ ] Diagonal Traversal
- [ ] Boundary Traversal
- [ ] In-place Modifications

---

### 17. Intervals
- [ ] Interval representation
- [ ] Sorting intervals
- [ ] Overlap detection

#### Problem Solving Patterns
- [ ] Merge Overlapping Intervals
- [ ] Insert Interval
- [ ] Interval Intersection
- [ ] Meeting Rooms (I & II)
- [ ] Non-overlapping Intervals
- [ ] Minimum Arrows to Burst Balloons
- [ ] Employee Free Time
- [ ] Interval Scheduling
- [ ] Range Module
- [ ] Sorting Intervals

---

### 18. Math & Geometry
- [ ] Basic number theory
- [ ] Geometric formulas
- [ ] Coordinate geometry

#### Problem Solving Patterns
- [ ] Prime Numbers (Sieve of Eratosthenes)
- [ ] GCD/LCM (Euclidean Algorithm)
- [ ] Modular Arithmetic
- [ ] Fast Exponentiation
- [ ] Factorial Problems
- [ ] Pascal's Triangle
- [ ] Rectangle Overlap
- [ ] Valid Square
- [ ] Line Intersection
- [ ] Angle Calculations

---

### 19. Design Problems
- [ ] Object-oriented design principles
- [ ] Interface design
- [ ] Time/space trade-offs

#### Problem Solving Patterns
- [ ] LRU Cache
- [ ] LFU Cache
- [ ] Design HashMap/HashSet
- [ ] Min Stack
- [ ] Design Twitter
- [ ] Implement Trie
- [ ] Design Search Autocomplete
- [ ] Design Hit Counter
- [ ] Design Logger Rate Limiter
- [ ] Design Circular Queue
- [ ] Design Tic-Tac-Toe
- [ ] Design Parking System

---

### 20. Advanced Structures (Optional)
- [ ] Advanced data structure basics
- [ ] When to use advanced structures

#### Problem Solving Patterns
- [ ] Segment Trees (range queries)
- [ ] Fenwick Tree/Binary Indexed Tree
- [ ] Suffix Arrays
- [ ] Sparse Tables
- [ ] Disjoint Set Union (DSU/Union-Find)
- [ ] AVL Trees
- [ ] Red-Black Trees
- [ ] Skip Lists
- [ ] B-Trees
- [ ] Bloom Filters

---

## Study Plan Priority

### Week 1 (Must Know)
- [ ] Arrays & Strings
- [ ] Hash Tables
- [ ] Two Pointers
- [ ] Sliding Window
- [ ] Stacks & Queues
- [ ] Binary Trees
- [ ] Binary Search

### Week 2 (Should Know)
- [ ] Linked Lists
- [ ] Graphs (BFS/DFS)
- [ ] Heaps
- [ ] Basic Dynamic Programming
- [ ] Backtracking basics

### Week 3+ (Nice to Know)
- [ ] Advanced DP patterns
- [ ] Greedy algorithms
- [ ] Bit Manipulation
- [ ] Tries
- [ ] Design problems

### Advanced (Company/Role Specific)
- [ ] Union Find
- [ ] Topological Sort
- [ ] Advanced graph algorithms
- [ ] Segment Trees
- [ ] Advanced DP variations