Problem: Remove Duplicates from Sorted Array (LeetCode #26)

Difficulty: Easy
Language: Java
Topic: Array, Two Pointers

Problem Statement:
Given an integer array nums sorted in non-decreasing order, remove the duplicates in-place such that each unique element appears only once.

The relative order of the elements should be kept the same.

Return the number of unique elements k.

To be accepted, the first k elements of nums should contain the unique elements.

Example:

Input: nums = [1,1,2]
Output: 2
Explanation:
After removing duplicates, the first 2 elements are [1,2].


Input: nums = [0,0,1,1,1,2,2,3,3,4]
Output: 5
Explanation:
After removing duplicates, the first 5 elements are [0,1,2,3,4].


Solution:

Handle the edge case where the array is empty.

Initialize a pointer i to track the position of unique elements.

Traverse the array using another pointer j.

If nums[j] is different from nums[i], increment i and assign nums[j] to nums[i].

Continue until all elements are processed.

Return i + 1 as the count of unique elements.
