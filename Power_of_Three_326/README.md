Problem: Power of Three (LeetCode #326)

Difficulty: Easy
Language: Java
Topic: Math

Problem Statement:
Given an integer n, return true if it is a power of three. Otherwise, return false.

An integer n is a power of three if there exists an integer x such that:

n = 3^x


Example:

Input: n = 27
Output: true

Explanation:
27 = 3 × 3 × 3 = 3^3

Input: n = 0
Output: false

Input: n = 9
Output: true


Solution:

If n <= 0, return false.

While n is divisible by 3, divide n by 3.

After the loop, check if n == 1.

If yes, it is a power of three; otherwise, return false.
