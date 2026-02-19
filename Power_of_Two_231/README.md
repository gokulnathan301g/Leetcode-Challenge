Problem: Power of Two (LeetCode #231)

Difficulty: Easy
Language: Java
Topic: Math, Bit Manipulation

Problem Statement:
Given an integer n, return true if it is a power of two. Otherwise, return false.

An integer n is a power of two if there exists an integer x such that:

n = 2^x


Example:

Input: n = 16
Output: true

Explanation:
16 = 2 × 2 × 2 × 2 = 2^4

Input: n = 3
Output: false

Input: n = 1
Output: true


Solution:

If n <= 0, return false.

While n > 1, check if n is divisible by 2.

If at any step n % 2 != 0, return false.

Divide n by 2 repeatedly.

If the loop ends and n == 1, return true.
