
# Longest Valid Parentheses

## Problem Statement

Given a string containing only '(' and ')',
find the length of the longest valid (well-formed)
parentheses substring.

## Approach: Stack

We use a stack to store the indices of parentheses.

1. Initialize the stack with -1 as the base index.
2. If the current character is '(', push its index.
3. If it is ')', pop the stack.
4. If the stack becomes empty, push the current index.
5. Otherwise, calculate the valid substring length:
   current index - stack top.
6. Update the maximum length.

## Complexity Analysis

- Time Complexity: O(n)
- Space Complexity: O(n)

Here, n is the length of the input string.

## Example 1

Input:
(() 

Output:
2

Explanation:
The longest valid substring is "()".

## Example 2

Input:
)()())

Output:
4

Explanation:
The longest valid substring is "()()".

## Technologies Used

- C++
- STL Stack
- String Processing
