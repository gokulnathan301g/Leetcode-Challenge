Problem: Reverse Prefix of Word (LeetCode #2000)

Difficulty: Easy
Language: Java
Topic: String

Problem Statement:
Given a 0-indexed string s and a character ch, reverse the segment of s that starts at index 0 and ends at the first occurrence of ch (inclusive).

If ch does not exist in s, return the original string.

Example:

Input: s = "abcdefd", ch = 'd'
Output: "dcbaefd"
Explanation:
The prefix up to the first 'd' is reversed.


Input: s = "xyxzxe", ch = 'z'
Output: "zxyxxe"
Explanation:
The prefix up to 'z' is reversed.


Input: s = "abcd", ch = 'z'
Output: "abcd"
Explanation:
Character not found, string remains unchanged.


Solution:

Find the index of the first occurrence of the given character.

Reverse the substring from index 0 to that position.

Append the remaining part of the string unchanged.

Return the resulting string.
