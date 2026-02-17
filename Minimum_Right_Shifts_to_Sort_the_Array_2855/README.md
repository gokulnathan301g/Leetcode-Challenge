Problem: Minimum Right Shifts to Sort the Array (LeetCode #2855)

Difficulty: Easy
Language: Java
Topic: Array, Simulation

Problem Statement:
You are given a 0-indexed array of distinct integers nums.

In one operation, you can perform a right shift, where the last element moves to the front.

Return the minimum number of right shifts required to make the array strictly increasing.
If it is not possible, return -1.

Example:

Input: nums = [3,4,5,1,2]
Output: 2

Explanation:
After 1 right shift -> [2,3,4,5,1]
After 2 right shifts -> [1,2,3,4,5]
The array becomes strictly increasing.

Input: nums = [1,3,5]
Output: 0

Explanation:
The array is already strictly increasing.


Solution:

Traverse the array and count how many times nums[i] > nums[(i+1) % n].

Store the index where this drop occurs.

If the count is 0, the array is already sorted → return 0.

If the count is 1, return n - index - 1.

If the count is greater than 1, it cannot be sorted using right shifts → return -1.
