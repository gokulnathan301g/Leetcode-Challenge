Problem: Smallest Even Multiple (LeetCode #2413)

Difficulty: Easy
Language: Java
Topic: Math

Problem Statement:
Given a positive integer n, return the smallest positive integer that is a multiple of both 2 and n.

Example:

Input: n = 5
Output: 10
Explanation:
The smallest number that is a multiple of both 2 and 5 is 10.


Input: n = 6
Output: 6
Explanation:
6 is already even, so it is the smallest multiple of both 2 and 6.


Solution:

Check if n is already an even number using n % 2 == 0.

If it is even, return n directly.

If it is odd, multiply n by 2.

Return the result as the smallest even multiple.
