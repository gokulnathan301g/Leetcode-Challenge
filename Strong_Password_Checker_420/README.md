Difficulty: Hard
Language: Java
Topic: String, Greedy

Problem Statement:
A password is considered strong if it satisfies the following conditions:

It has at least 6 characters and at most 20 characters.

It contains at least one lowercase letter, one uppercase letter, and one digit.

It does not contain three repeating characters in a row (e.g., "aaa").

Given a string s, return the minimum number of steps required to make the password strong.
In one step, you can insert, delete, or replace a character.

Example:

Input: s = "a"
Output: 5
Explanation:
The password must be at least 6 characters long and must include
an uppercase letter and a digit.


Input: s = "aA1"
Output: 3
Explanation:
Insert characters to reach the minimum length.


Input: s = "1337C0d3"
Output: 0
Explanation:
The password already satisfies all the conditions.
