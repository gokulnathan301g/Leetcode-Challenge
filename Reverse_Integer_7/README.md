Problem: Reverse Integer (LeetCode #7)

Difficulty: Medium
Language: Java
Topic: Math

Problem Statement:
Given a signed 32-bit integer x, return x with its digits reversed.

If reversing x causes the value to go outside the signed 32-bit integer range
[-2³¹, 2³¹ - 1], then return 0.

Assume the environment does not allow storing 64-bit integers.

Example:

Input: x = 123
Output: 321


Input: x = -123
Output: -321


Input: x = 120
Output: 21


Solution:

Initialize a variable rev = 0 to store the reversed number.

Extract the last digit using x % 10.

Before updating rev, check for overflow conditions.

Multiply rev by 10 and add the extracted digit.

Remove the last digit from x using x /= 10.

Continue until x becomes 0.

Return the reversed integer, or 0 if overflow occurs.
