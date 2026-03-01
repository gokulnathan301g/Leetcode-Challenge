Problem: Minimum Operations to Make All Elements Divisible by 3

Difficulty: Easy
Language: Java
Topic: Math, Greedy, Modulo

📝 Problem Statement:

You are given an integer array nums.

In one operation, you can either:

Increment an element by 1, or

Decrement an element by 1

Return the minimum number of operations required to make every element in the array divisible by 3.

💡 Example:
Input: nums = [1,2,3,4]
Output: 3
Explanation:

For each number:

1 → needs 1 operation (1 → 0 or 3)

2 → needs 1 operation (2 → 3)

3 → needs 0 operations

4 → needs 1 operation (4 → 3)

Total = 3 operations

🚀 Solution Approach:

Initialize result = 0

For each number:

Compute remainder = num % 3

If remainder is 1 → 1 operation needed

If remainder is 2 → 1 operation needed

Add min(remainder, 3 - remainder) to result

Return total result
