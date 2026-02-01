Problem: Sqrt(x) (LeetCode #69)

Difficulty: Easy
Language: Java
Topic: Binary Search

Problem Statement:
Given a non-negative integer x, return the square root of x rounded down to the nearest integer.
The returned integer should be non-negative as well.

You must not use any built-in exponent function or operator.

Example:

Input: x = 4
Output: 2
Explanation: The square root of 4 is 2.


Input: x = 8
Output: 2
Explanation: The square root of 8 is approximately 2.828,
so the result is rounded down to 2.


Solution:

Handle base cases where x is 0 or 1.

Use binary search between 1 and x.

Calculate mid and check mid * mid using long to avoid overflow.

If mid * mid is less than or equal to x, store mid as a possible answer.

Adjust search boundaries accordingly.

Return the stored answer as the integer square root.
