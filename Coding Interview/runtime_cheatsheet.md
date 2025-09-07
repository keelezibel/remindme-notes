## O(1)
- Hashmap lookup
- Array access and update
- Stack push and pop
- Finding and applying math formula
- Typically for n > 10<sup>9</sup>

## O(log n)
- Binary search
- Lookup by primary key in relational DB (e.g. B-tree searching in Postgres)
- Typically for n > 10<sup>8</sup>

## O(n)
Looping through linear data structure
- Going through array, linked list, string
- Two pointers
- Tree/Graph traversal
- Stack/Queue traversal
- Typically for n <= 10<sup>6</sup>

## O(k log n)
- Heap push/pop (k times)
- Binary search (k times)
- Typically for n <= 10<sup>6</sup>

## O(n log n)
- Efficient sorting algorithms (e.g. Merge Sort, Quick Sort, Heap Sort)
- Divide and conquer algorithms (divide is O(log N) and merge is O(N))
- Typically for n <= 10<sup>6</sup>

## O(n<sup>2</sup>) quadratic
- Nested loops
- Brute force
- N <= 3000

## O(2<sup>n</sup>) exponential
- Often need memoization or pruning to optimize
- N <= 20

## O(n!)
- Generating all permutations
- N <= 12