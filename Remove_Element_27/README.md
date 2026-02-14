Problem: Remove Element (LeetCode #26)

Difficulty: Easy
Language: Java
Topic: Array, Two Pointers

Problem Statement:
Given an integer array nums and an integer val, remove all occurrences of val in-place.

The relative order of the elements may be changed.
Return the number of elements in nums which are not equal to val.

Consider the number of elements not equal to val as k.
To be accepted, the first k elements of nums should contain the elements not equal to val.

Example:

Input: nums = [3,2,2,3], val = 3
Output: 2
Explanation:
After removing 3, the first 2 elements are [2,2].


Input: nums = [0,1,2,2,3,0,4,2], val = 2
Output: 5
Explanation:
After removing 2, the first 5 elements are [0,1,4,0,3].


Solution:

Initialize a counter k = 0 to track the position of valid elements.

Traverse the array from index 0 to the end.

If the current element is not equal to val, assign it to nums[k] and increment k.

Continue until all elements are processed.

Return k as the count of elements not equal to val.
