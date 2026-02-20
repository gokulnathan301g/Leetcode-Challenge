Problem: Plus One (LeetCode #66)

Difficulty: Easy
Language: Java
Topic: Array, Math

Problem Statement:
You are given a large integer represented as an integer array digits, where each digits[i] is a single digit.

The digits are ordered from most significant to least significant.

Increment the large integer by one and return the resulting array of digits.

Example:

Input: digits = [1,2,3]
Output: [1,2,4]

Explanation:
123 + 1 = 124
Input: digits = [9]
Output: [1,0]
Input: digits = [9,9,9]
Output: [1,0,0,0]

Solution:

Start from the last digit and initialize carry = 1 (since we are adding one).

Add carry to the current digit.

Update the digit as sum % 10 and update carry as sum / 10.

If carry becomes 0, stop early and return the modified array.

If carry remains after processing all digits, create a new array of size n + 1.

Set the first element to 1 and copy the remaining digits.
