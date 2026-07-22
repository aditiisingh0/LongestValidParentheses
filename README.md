# Longest Valid Parentheses

## Problem
Given a string containing only '(' and ')', return the length of the longest valid parentheses substring.

## Approach
- Use a stack to store indices.
- Initialize the stack with `-1`.
- Push indices of '('.
- For ')', pop the stack.
- If the stack becomes empty, push the current index.
- Otherwise, calculate the valid substring length as `currentIndex - stack.peek()`.

## Complexity
- Time: O(n)
- Space: O(n)

## Example
Input: "(()"
Output: 2

Input: ")()())"
Output: 4

Input: ""
Output: 0
