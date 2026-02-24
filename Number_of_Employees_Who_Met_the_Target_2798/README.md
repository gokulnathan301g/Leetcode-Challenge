Problem: Number of Employees Who Met the Target (LeetCode #2798)

Difficulty: Easy
Language: Java
Topic: Array, Counting

Problem Statement:
There are n employees in a company, numbered from 0 to n - 1.

You are given a 0-indexed integer array hours of length n where hours[i] is the number of hours worked by the i-th employee.

You are also given an integer target.

Return the number of employees who worked at least target hours.

Example:

Input: hours = [0,1,2,3,4], target = 2
Output: 3

Explanation:
Employees with hours ≥ 2 are:
2, 3, 4 → Total = 3
Input: hours = [5,1,4,2,2], target = 6
Output: 0

Solution:

Initialize a counter total = 0.

Traverse through each element in hours.

If hours[i] >= target, increment total.

Return total.
