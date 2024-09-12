# Quicksort and Hash Table Implementation

This project contains implementations of Randomized Quicksort, Deterministic Quicksort, and a Hash Table, along with an analysis of their performance.

## How to Run the Code

### Part 1: Quicksort

1. Ensure you have Python installed on your system.
2. Open a terminal or command prompt.
3. Navigate to the directory containing `part1.py`.
4. Run the script using the command:
   ```
   python part1.py
   ```
5. The script will output the sorted array and the execution times for both Randomized and Deterministic Quicksort.

### Part 2: Hash Table

1. Navigate to the directory containing `part2.py`.
2. Run the script using the command:
   ```
   python part2.py
   ```
3. The script will demonstrate the basic operations of the Hash Table implementation.

## Summary of Findings

### Part 1: Quicksort Analysis

1. **Time Complexity:**
   - Both Randomized and Deterministic Quicksort have an average-case time complexity of O(n log n).
   - Randomized Quicksort helps prevent worst-case scenarios (O(n^2)) that can occur in Deterministic Quicksort.

2. **Performance Comparison:**
   - For an array of 1000 elements, both algorithms performed similarly, with Deterministic Quicksort being slightly faster.
   - The overhead of random number generation in Randomized Quicksort may account for the small time difference in small datasets.

3. **Input Distribution Effects:**
   - Randomized Quicksort is more robust against already sorted, reverse sorted, or arrays with many duplicates.
   - Deterministic Quicksort can degrade to O(n^2) for sorted or reverse sorted arrays.

### Part 2: Hash Table Analysis

1. **Time Complexity:**
   - Expected time complexity for insert, search, and delete operations is O(1) under simple uniform hashing.
   - Worst-case time complexity can degrade to O(n) if many elements hash to the same index.

2. **Load Factor:**
   - The load factor (α = n/m) significantly influences the hash table's performance.
   - A lower load factor results in faster operations due to shorter chains.

3. **Strategies for Efficiency:**
   - Dynamic resizing: Increase table size when the load factor exceeds a threshold.
   - Universal hashing: Use a family of hash functions to distribute keys evenly.
   - Prime number table size: Reduces clustering of hash values.

These implementations and analyses demonstrate the importance of algorithm choice and data structure design in achieving optimal performance for different scenarios.
