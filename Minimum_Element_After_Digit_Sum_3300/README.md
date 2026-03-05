Problem: Minimum Element After Replacement With Digit Sum (LeetCode #3300)

Difficulty: Easy
Language: Java
Topic: Math, Array, Digit Manipulation

📝 Problem Statement:

You are given an integer array nums.

For each number in the array, replace it with the sum of its digits.

Return the minimum element in the resulting array.

💡 Example:
Input:
nums = [10,12,13,14]

Output:
1
Explanation:

Compute digit sums:

10 → 1 + 0 = 1
12 → 1 + 2 = 3
13 → 1 + 3 = 4
14 → 1 + 4 = 5

New array → [1,3,4,5]

Minimum element = 1

🚀 Solution Approach:

Initialize min = Integer.MAX_VALUE.

Traverse each number in the array.

Compute the digit sum using:

n % 10 to extract digits

n / 10 to remove digits

Update min with the smallest digit sum found.

Return min.
