Problem: Reverse String (LeetCode #344)

Difficulty: Easy
Language: Java
Topic: String, Two Pointers

Problem Statement:
Write a function that reverses a string.
The input string is given as an array of characters s.

You must do this by modifying the input array in-place with O(1) extra memory.

Example:

Input: s = ["h","e","l","l","o"]
Output: ["o","l","l","e","h"]
Explanation:
Characters are swapped from both ends.


Input: s = ["H","a","n","n","a","h"]
Output: ["h","a","n","n","a","H"]
Explanation:
The string is reversed in-place.


Solution:

Initialize two pointers: left at the start and right at the end of the array.

While left is less than right, swap the characters at these positions.

Move left forward and right backward after each swap.

Continue until the entire array is reversed.

The string is reversed in-place without using extra memory.
