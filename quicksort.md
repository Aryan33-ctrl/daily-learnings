
dixit@lappy MINGW64 ~
$ cd daily-learnings

dixit@lappy MINGW64 ~/daily-learnings (main)
$ nano quicksort.md

dixit@lappy MINGW64 ~/daily-learnings (main)
$ git add .

dixit@lappy MINGW64 ~/daily-learnings (main)
$ git commit -m "quick sort "
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

dixit@lappy MINGW64 ~/daily-learnings (main)
$ ^C

dixit@lappy MINGW64 ~/daily-learnings (main)
$ ls
2026-01-24.md                         daily-learning.md.save.1
Day-4-Searching.md                    daily-learnings.md
DAY XX – DSA LEARNING
TOPIC: QUICK SORT

1. WHAT IS QUICK SORT
Quick Sort is a Divide and Conquer sorting algorithm.
It selects a pivot element and partitions the array into:
- elements smaller than pivot
- elements greater than pivot
Then it recursively sorts both parts.

--------------------------------------------------

2. WORKING STEPS
1. Choose a pivot element (usually last element).
2. Rearrange array so smaller elements come before pivot
   and larger elements come after pivot.
3. Place pivot at correct sorted position.
4. Apply Quick Sort recursively on left and right subarrays.

--------------------------------------------------

3. IS QUICK SORT RECURSIVE?
Yes.
Quick Sort uses recursion because it repeatedly divides
the array into smaller subproblems.

--------------------------------------------------

4. TIME COMPLEXITY
Best Case:    O(n log n)
Average Case: O(n log n)
Worst Case:   O(n^2)   (when array already sorted and bad pivot chosen)

--------------------------------------------------

5. SPACE COMPLEXITY
O(log n) due to recursion stack.

--------------------------------------------------

6. ADVANTAGES
- Very fast in practice.
- Efficient for large datasets.
- In-place sorting (no extra array needed).
- Cache friendly.
- Widely used in real-world systems.

--------------------------------------------------

7. DISADVANTAGES
- Worst case O(n^2).
- Not a stable sorting algorithm.
- Recursive calls may cause stack overflow
  for very large arrays.

--------------------------------------------------

8. WHERE QUICK SORT IS USED
- System level sorting
- Large data processing
- Programming libraries
- Competitive programming

--------------------------------------------------

9. KEY CONCEPTS LEARNED
- Divide and Conquer
- Recursion
- Partition Algorithm
- Pivot Selection
- In-place sorting

--------------------------------------------------

10. DRY RUN EXAMPLE
Array: [5,2,9,1,3]
Pivot = 3

After partition:
[2,1] 3 [5,9]

Sort left -> [1,2]
Sort right -> [5,9]

Final sorted array:
[1,2,3,5,9]

--------------------------------------------------

LEARNING SUMMARY
Today I learned Quick Sort algorithm including
its working, recursion usage, advantages,
disadvantages, time complexity, and practical uses.

