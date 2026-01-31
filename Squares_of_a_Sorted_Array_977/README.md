Problem: Squares of a Sorted Array (LeetCode #977)

Difficulty: Easy
Language: Java
Topic: Array, Sorting

Problem Statement:
Given an integer array nums sorted in non-decreasing order, return an array of the squares of each number, also sorted in non-decreasing order.

Example:

Input: nums = [-4, -1, 0, 3, 10]
Squares = [16, 1, 0, 9, 100]
Output: [0, 1, 9, 16, 100]


Input: nums = [-7, -3, 2, 3, 11]
Squares = [49, 9, 4, 9, 121]
Output: [4, 9, 9, 49, 121]


Solution:

Traverse the array and square each element.

Store the squared values back into the same array.

Sort the array using a built-in sorting method.

Return the sorted squared array.
