Problem: Palindrome Number (LeetCode #9)

Difficulty: Easy
Language: Java
Topic: Math, Two Pointers

Problem Statement:
Given an integer x, return true if x is a palindrome, and false otherwise.

An integer is a palindrome when it reads the same backward as forward.

Example:

Input: x = 121
Output: true

Explanation:
121 reads the same from left to right and right to left.
Input: x = -121
Output: false

Explanation:
From left to right, it reads -121.
From right to left, it becomes 121-.
Input: x = 10
Output: false

Solution:

If x < 0, return false since negative numbers cannot be palindromes.

Convert the integer to a string.

Use two pointers:

left starting at index 0

right starting at the last index

Compare characters at left and right.

If any mismatch occurs, return false.

Move pointers inward until they meet.

If all characters match, return true.
