Problem: Apple Redistribution into Boxes (LeetCode #3074)

Difficulty: Easy
Language: Java
Topic: Greedy, Sorting, Arrays

📝 Problem Statement:

You are given two integer arrays:

apple → number of apples in each pile

capacity → capacity of each box

Each box can hold up to its capacity of apples.

Return the minimum number of boxes required to store all apples.

💡 Example:
Input:
apple = [1,3,2]
capacity = [4,3,1,5,2]

Output:
2
Explanation:

Total apples =
1 + 3 + 2 = 6

Sort capacities:
[1,2,3,4,5]

Pick largest boxes first:

5 → remaining apples = 1
4 → remaining apples = -3

Only 2 boxes needed.

🚀 Solution Approach:

Calculate total apples.

Sort capacity array.

Start picking boxes from the largest capacity.

Keep adding capacities until the sum ≥ total apples.

Return number of boxes used.
