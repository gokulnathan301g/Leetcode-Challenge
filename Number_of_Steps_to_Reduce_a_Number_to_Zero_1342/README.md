Problem: Number of Steps to Reduce a Number to Zero (LeetCode #1342)

Difficulty: Easy
Language: Java
Topic: Math, Simulation

Problem Statement:
Given an integer num, return the number of steps to reduce it to zero.

In one step:

If the current number is even, divide it by 2.

If the current number is odd, subtract 1 from it.

Continue until num becomes 0.

Example:

Input: num = 14
Output: 6

Explanation:
14 → 7 → 6 → 3 → 2 → 1 → 0
Total steps = 6
Input: num = 8
Output: 4
Input: num = 123
Output: 12

Solution:

Initialize a counter step = 0.

While num > 0:

If num is even, divide it by 2.

Otherwise, subtract 1.

Increment step.

Return step.
