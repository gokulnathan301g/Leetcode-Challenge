Problem: Separate the Digits in an Array (LeetCode #2553)

Difficulty: Easy
Language: Java
Topic: Array, Math

Problem Statement:
Given an array of positive integers nums, return an array digits where each element of nums is split into its individual digits in the same order they appear.

Example:

Input: nums = [13,25,83,77]
Output: [1,3,2,5,8,3,7,7]
Explanation:
Each number is broken into digits and added in order.


Input: nums = [7,1,3,9]
Output: [7,1,3,9]
Explanation:
Each number already consists of a single digit.


Solution:

Traverse the array to calculate the total number of digits required.

Create a result array with the calculated size.

Traverse the original array from the end to preserve digit order.

Extract digits using % 10 and place them in the result array.

Continue until all numbers are fully processed.

Return the final digits array.
