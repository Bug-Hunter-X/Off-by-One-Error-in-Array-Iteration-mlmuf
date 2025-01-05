# Off-by-One Error in Array Iteration
This repository demonstrates a common off-by-one error in Java. The code attempts to iterate through an array, but due to an error in the loop condition, it tries to access an index that is out of bounds. 

## Bug Description
The `Bug.java` file contains a for loop that iterates from 0 up to and *including* `arr.length`.  Since array indices are zero-based, the last valid index is `arr.length - 1`. Accessing `arr[arr.length]` throws an `ArrayIndexOutOfBoundsException`. 

## Bug Solution
The solution is provided in `BugSolution.java`. The for loop condition is corrected to `i < arr.length` which correctly iterates through all valid array elements. 