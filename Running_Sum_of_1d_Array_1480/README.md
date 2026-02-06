Problem: Running Sum of 1d Array (LeetCode #1480)

Difficulty: Easy
Language: Java
Topic: Array, Prefix Sum

Problem Statement:
Given an array nums, return the running sum of nums.

The running sum at index i is the sum of all elements from index 0 to i (inclusive).

Example:

Input: nums = [1,2,3,4]
Output: [1,3,6,10]
Explanation:
Running sum is calculated as:
[1, 1+2, 1+2+3, 1+2+3+4]


Input: nums = [1,1,1,1,1]
Output: [1,2,3,4,5]


Solution:

Create a new array to store the running sum.

Set the first element equal to the first element of nums.

Traverse the array starting from index 1.

At each index, add the current value to the previous running sum.

Store the result in the running sum array.

Return the final running sum array.
