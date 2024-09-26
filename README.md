# Recursion
Experiment_15

## Contents
- [Aim](#aim)
- [Software Used](#software-used)
- [Theory](#theory)
  * [Definition](#Definition)
  * [Properties](#Properties-of-recursion)
  * [Advantages](#Advantages-of-recusion)
- [Algorithms](#algorithms)
- [Conclusion](#conclusion)

## Aim: 
To Study and Implement Recursion Function.

## Software Used:
VS Code , Dev C++

## Theory:
Assume that you have to paint a few balls. If you do it alone, it will take a lot of time. One thing you can do is to take help from your friend. Assuming that you have the same work speed, the task will be done in half of the time. Now, instead of taking help from only one of your friends, you take help from multiple friends such that each friend have only one ball to paint. The task will be done much faster as compared to when you were doing it alone. Recursion is a problem-solving technique that works in a similar way.
Recursion in C++ is a technique in which a function calls itself repeatedly until a given condition is satisfied. In other words, recursion is the process of solving a problem by breaking it down into smaller, simpler sub-problems.

## Syntax Structure of Recursion
return_type recursive_func {
    ....
       // Base Condition
       // Recursive Case
       ....
}

### Properties of Recursion:
Recursion is a programming technique where a function calls itself to solve a problem. Here are some key properties and advantages of recursion:

### Properties of Recursion
1. **Base Case**: Every recursive function must have a base case to terminate the recursion and prevent infinite loops. This is the simplest instance of the problem that can be solved directly.
2. **Recursive Case**: The function breaks down the problem into smaller subproblems, calling itself to solve those.
3. **Stack Memory**: Each recursive call is added to the call stack, which holds the state of each function call until it completes.
4. **Problem Decomposition**: Recursion naturally breaks problems into smaller, more manageable parts, making it easier to implement solutions for complex problems.

### Advantages of Recursion
1. **Simplicity and Clarity**: Recursive solutions can be more straightforward and easier to understand than their iterative counterparts, especially for problems like tree traversal and factorial calculations.
2. **Elegant Solutions**: Many algorithms (like quicksort and mergesort) are elegantly expressed using recursion, leading to cleaner and more concise code.
3. **Reduced Code Length**: Recursive implementations can be shorter and less complex than iterative ones, reducing potential errors in logic and making the code easier to maintain.
4. **Natural Fit for Certain Problems**: Problems that exhibit self-similarity, such as traversing trees or solving combinatorial problems (like the Fibonacci sequence), often lend themselves well to recursion.
5. **Ease of Backtracking**: Recursion is particularly useful in problems that require exploring multiple possibilities, such as pathfinding in mazes or generating permutations.
6. **Functional Programming Compatibility**: Many functional programming languages emphasize recursion as a primary control structure, making it a fundamental concept in those paradigms.

### Algorithm for Calculating Factorial

1. **Start**: Begin the program.
2. **Input**: Prompt the user to enter a number \( n \).
3. **Function Definition**: Define a recursive function `factorial(n)`:
   - **Base Case**: If \( n \) is less than or equal to 1:
     - Return 1.
   - **Recursive Case**: Otherwise:
     - Return \( n \times \) `factorial(n - 1)`.
4. **Call Function**: In the `main` function, call `factorial(num)` with the user input.
5. **Output**: Display the result of the factorial calculation.
6. **End**: Terminate the program.

### Algorithm for reverse string:

1. **Input the String:**
   - Prompt the user to enter a string.
   - Store the string in a character array.
2. **Reverse the String Using Recursion:**
   - Define a recursive function `rev` that takes a character pointer (the string).
   - If the current character pointed to is not the null terminator (`'\0'`):
     - Call the `rev` function recursively with the next character (i.e., move to the next index).
     - After returning from the recursive call, print the current character.
3. **Output the Result:**
   - Call the `rev` function from the `main` function to initiate the reversal.
   - Print a newline after displaying the reversed string.

### Algorithm for reverse integer:

1. **Input the Number:**
   - Prompt the user to enter an integer.
   - Read and store the integer in a variable (`num`).
2. **Define the Recursive Function (`rev`):**
   - The function takes an integer `i` as a parameter.
   - **Base Case:** If `i` is greater than 0:
     - Print the last digit of `i` using `i % 10`.
     - Call the `rev` function with the integer divided by 10 (`i / 10`).
3. **Output the Result:**
   - Call the `rev` function with the input number.
   - Print a newline after displaying the reversed number.

### Algorithm Sum of integers:

1. **Input the Number:**
   - Prompt the user to enter an integer.
   - Read and store the integer in a variable (`num`).

2. **Define the Recursive Function (`sum`):**
   - The function takes an integer `n` as a parameter.
   - **Base Case:** If `n` is equal to 0, return 0.
   - **Recursive Case:** Return the sum of `n` and the result of calling `sum` with `n - 1`.

3. **Output the Result:**
   - Call the `sum` function with the input number.
   - Print the result, which is the sum of integers from 1 to `num`.

## Conclusion:
We learnt to use the concepts of recursion and used in the programs for factorial,reverse string,reverse integer and sum of integers.


   

