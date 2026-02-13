Problem: Remove Outermost Parentheses (LeetCode #1021)

Difficulty: Easy
Language: Java
Topic: String, Stack / Depth Counting

Problem Statement:
A valid parentheses string is either empty "", "(" + A + ")", or A + B,
where A and B are valid parentheses strings.

Given a valid parentheses string s, remove the outermost parentheses of every primitive string and return the result.

A primitive valid parentheses string is a non-empty string that can be written as A,
and cannot be split into A = B + C, where B and C are non-empty valid parentheses strings.

Example:

Input: s = "(()())(())"
Output: "()()()"
Explanation:
The string can be decomposed into "(()())" + "(())".
Removing outer parentheses from each gives "()()" + "()"


Input: s = "(()())(())(()(()))"
Output: "()()()()(())"


Input: s = "()()"
Output: ""


Solution:

Initialize a variable depth = 0 to track nesting level.

Traverse each character in the string.

When encountering '(', append it only if depth > 0, then increment depth.

When encountering ')', decrement depth first, then append it only if depth > 0.

Continue until all characters are processed.

Return the constructed string without outermost parentheses.
