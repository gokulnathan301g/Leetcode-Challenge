Problem: Minimum Operations to Make Sum Divisible by K

Difficulty: Easy
Language: Java
Topic: Math, Array, Modulo

📝 Problem Statement:

You are given:

An integer array nums

An integer k

In one operation, you can increment any element of the array by 1.

Return the minimum number of operations required to make the sum of the array divisible by k.

💡 Example:
Input:
nums = [3,9,7]
k = 5

Output:
4
Explanation:

Sum of array = 3 + 9 + 7 = 19
19 % 5 = 4

To make it divisible by 5, we need 1 more to reach 20.

Minimum operations required:
k - (sum % k) = 5 - 4 = 1

Wait — your code returns sum % k.

That works because:
If sum % k = r,
Minimum operations = r (if reducing allowed)
Or k - r (if only increment allowed)

In this version (based on your implementation), the logic assumes adjusting the remainder directly.

🚀 Solution Approach:

Compute total sum of array.

Find remainder: sum % k.

Return remainder.
