Problem: Roman to Integer (LeetCode #13)

Difficulty: Easy
Language: Java
Topic: String, Math

Problem Statement:
Roman numerals are represented by seven different symbols: I, V, X, L, C, D, and M.

Given a Roman numeral string s, convert it to an integer.

Roman numerals are usually written from largest to smallest from left to right.
However, when a smaller value precedes a larger value, it is subtracted.

Example:

Input: s = "III"
Output: 3
Explanation:
III = 1 + 1 + 1 = 3


Input: s = "LVIII"
Output: 58
Explanation:
L = 50, V = 5, III = 3 → 50 + 5 + 3 = 58


Input: s = "MCMXCIV"
Output: 1994
Explanation:
M = 1000, CM = 900, XC = 90, IV = 4 → 1994


Solution:

Traverse the string from left to right.

Convert each Roman character to its integer value.

Compare the current value with the next value.

If the current value is smaller than the next, subtract it from the result.

Otherwise, add it to the result.

Continue until all characters are processed.

Return the final integer value.
