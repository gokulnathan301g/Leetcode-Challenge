Problem: Number of Good Pairs (LeetCode #1512)

Difficulty: Easy
Language: Java
Topic: Array, Brute Force

Problem Statement:
Given an array of integers nums, return the number of good pairs.

A pair (i, j) is called good if:

nums[i] == nums[j]

i < j

Example:

Input: nums = [1,2,3,1,1,3]
Output: 4

Explanation:
The good pairs are:
(0,3), (0,4), (3,4), (2,5)
Input: nums = [1,1,1,1]
Output: 6
Input: nums = [1,2,3]
Output: 0

Solution:

Initialize a counter count = 0.

Use two nested loops:

Outer loop runs from 0 to n-1

Inner loop runs from i+1 to n-1

If nums[i] == nums[j], increment count.

Return count.
