Difficulty: Easy
Language: Java
Topic: Math

Problem Statement:
Given an integer n, return the value obtained by subtracting the sum of its digits from the product of its digits.

Example:

Input: n = 234
Product = 2 * 3 * 4 = 24
Sum = 2 + 3 + 4 = 9
Output: 15

Explanation: 24 - 9 = 15


Input: n = 4421
Product = 4 * 4 * 2 * 1 = 32
Sum = 4 + 4 + 2 + 1 = 11
Output: 21


Solution:

Initialize prod = 1 and sum = 0.

Extract each digit using n % 10.

Add the digit to sum and multiply it with prod.

Remove the last digit using n /= 10.

Finally return prod - sum.
