# Problem Solving

Many of these strategies are adapted from George Polya's book *How to Solve It* 

## Steps for solving problems
### 1. Understand the Problems

    1. Can I restate the problem in my own words
    2. What inputs go into the problem
    3. What are the outputs that should come from the solution
    4. Can the outputs be determined from the inputs
    5. How should I label important pieces of data (variable names and such)

### 2. Explore Concrete Examples

    1. Write down 2-3 simple examples
    2. Progress to more complex examples
    3. Explore examples with empty inputs
    4. Explore examples with invalid inputs

### 3. Break It Down

    1. Explicitly write the steps you need to take (makes you catch conceptual ideas or misunderstandings before diving in)

        • Put simply

            ```javascript
                function charCount(str) {
                    // create object to return at end
                    // loop over string for each character...
                        // if char is a number / letter && is a key in object, add one to count
                        // if the char is a number / letter && not in object, add it to obj and set value to 1
                        // if char is something else, do nothing (space, punctuation)
                    // return object at end
                }
            ```

### 4. Solve / Simplify (if you can't, solve a simpler problem)

    * Find the core difficulty in what you're trying to do
    * Temporarily ignore that difficulty
    * Write a simplified solution
    * Then incorporate difficulty back in

### 5. Look Back and Refactor

    * Can you check the result?
    * Can you derive the result differently?
    * Can you understand it at a glance?
    * Can you use the result or method for some other problem?
    * Can you improve the performance of the solution?
    * Can you think of other ways to refactor?
    * How have other people solved this problem?

---
## Eight Must-Know Algorithms for Coding Interviews

### 1. Data Structure Manipulation

### 2. Searching (depth-first & breadth-first)
    * Word Ladder Problem

### 3. Combinations & Permutations
    * Zero One Knapsack Problem

### 4. Sort (quick, merge, insertion, etc.)
    * How to sort arbitrary data structures

### 5. Binary Search
    * In rotated array, find the pivot point

### 6. Topological Sort
    * Useful when looking at graph problems 
    * When trying to order data based on any sort of restrictions

### 7. Recursion (http://byte-by-byte.com/recursion)

### 8. Dynamic Programming (http://dynamicprogrammingbook.com)
