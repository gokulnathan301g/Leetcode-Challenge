Problem: Special Array I (LeetCode #3151)

Difficulty: Easy
Language: Java
Topic: Array

Problem Statement:
An array is considered special if the parity (even or odd) of every pair of adjacent elements is different.

Given an integer array nums, return true if the array is special. Otherwise, return false.

Example:

Input: nums = [1]
Output: true
Explanation:
A single-element array is always special.


Input: nums = [2, 1, 4]
Output: true
Explanation:
Even → Odd → Even (parity alternates).


Input: nums = [4, 3, 1]
Output: false
Explanation:
Odd and Odd appear consecutively.


Solution:

Traverse the array from index 0 to n - 2.

Compare the parity of the current element and the next element using % 2.

If two adjacent elements have the same parity, return false.

If all adjacent elements alternate in parity, return true.
