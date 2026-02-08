Problem: Robot Return to Origin (LeetCode #657)

Difficulty: Easy
Language: Java
Topic: String, Simulation

Problem Statement:
There is a robot starting at position (0, 0), the origin, on a 2D plane.
Given a string moves, where each character represents a move made by the robot:

'U' → move up

'D' → move down

'L' → move left

'R' → move right

Return true if the robot returns to the origin after completing all moves. Otherwise, return false.

Example:

Input: moves = "UD"
Output: true
Explanation:
The robot moves up and then down, returning to the origin.


Input: moves = "LL"
Output: false
Explanation:
The robot moves left twice and does not return to the origin.


Input: moves = "URDL"
Output: true
Explanation:
All movements cancel each other out.


Solution:

Initialize two variables x and y to track the robot’s position.

Traverse each character in the moves string.

Update x and y based on the move direction.

After processing all moves, check if both x and y are 0.

Return true if the robot is back at the origin, otherwise return false.
