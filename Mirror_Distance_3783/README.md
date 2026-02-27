Problem: Difference Between Element Sum and Digit Sum of an Array (Mirror Distance Logic Variant)

Difficulty: Easy
Language: Java
Topic: Math, Number Manipulation

Problem Statement:
Given an integer n, reverse its digits and compute the absolute difference between the original number and the reversed number.

Return the absolute difference.

Example:
Input: n = 25
Output: 27

Explanation:
Original = 25
Reversed = 52
|25 - 52| = 27
Input: n = 10
Output: 9
Solution Approach:

Store the original number.

Reverse the number using:

Extract last digit → n % 10

Build reversed number → rev = rev * 10 + digit

Remove last digit → n = n / 10

Return Math.abs(original - rev).
