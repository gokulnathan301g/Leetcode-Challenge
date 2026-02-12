Problem: Replace Elements with Greatest Element on Right Side (LeetCode #1299)

Difficulty: Easy
Language: Java
Topic: Array

Problem Statement:
Given an array arr, replace every element in that array with the greatest element among the elements to its right, and replace the last element with -1.

After doing so, return the array.

Example:

Input: arr = [17,18,5,4,6,1]
Output: [18,6,6,6,1,-1]
Explanation:
- 17 → greatest on right is 18  
- 18 → greatest on right is 6  
- 5 → greatest on right is 6  
- 4 → greatest on right is 6  
- 6 → greatest on right is 1  
- 1 → -1 (last element)


Solution:

Initialize a variable max as -1 to track the maximum element from the right.

Traverse the array from right to left.

Store the current element before updating it.

Replace the current element with max.

Update max if the stored value is greater than the current max.

Continue until the beginning of the array.

Return the modified array.
