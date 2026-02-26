Problem: Move Zeroes (LeetCode #283)

Difficulty: Easy
Language: Java
Topic: Array, Two Pointers

Problem Statement:
Given an integer array nums, move all 0's to the end of it while maintaining the relative order of the non-zero elements.

You must do this in-place without making a copy of the array.

Example:

Input: nums = [0,1,0,3,12]
Output: [1,3,12,0,0]
Input: nums = [0]
Output: [0]
Solution Approach:

Initialize a pointer index = 0.

Traverse the array:

If nums[i] != 0, place it at nums[index] and increment index.

After placing all non-zero elements, fill the remaining positions with 0.
