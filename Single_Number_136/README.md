Problem: Single Number (LeetCode #136)

Difficulty: Easy
Language: Java
Topic: Array, Bit Manipulation

Problem Statement:
Given a non-empty array of integers nums, every element appears twice except for one.
Find that single one.

You must implement a solution with linear runtime complexity and constant extra space.

Example:

Input: nums = [2,2,1]
Output: 1
Explanation:
The element 1 appears only once.


Input: nums = [4,1,2,1,2]
Output: 4
Explanation:
The element 4 appears only once.


Solution:

Initialize a variable ans to 0.

Traverse through the array elements.

Apply the XOR (^) operation between ans and each element.

Since a ^ a = 0 and a ^ 0 = a, all duplicate numbers cancel out.

The remaining value in ans is the single number.

Return ans.
