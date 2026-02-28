Problem: Minimum Processing Time (LeetCode #2895)

Difficulty: Medium
Language: Java
Topic: Greedy, Sorting, Arrays

📝 Problem Statement:

You are given:

A list processorTime where processorTime[i] represents the time taken by the i-th processor.

A list tasks where each task has a processing time.

Each processor must handle exactly 4 tasks.

The time taken by a processor is:

processorTime[i] + max(task time assigned to that processor)

Return the minimum possible maximum processing time among all processors.

💡 Example:
Input:
processorTime = [8, 10]
tasks = [2,2,3,1,8,7,4,5]

Output:
16
Explanation:

Sort processorTime in ascending order → [8,10]

Sort tasks in descending order → [8,7,5,4,3,2,2,1]

Assign 4 largest remaining tasks per processor

Processor 1 → 8 + 8 = 16
Processor 2 → 10 + 3 = 13

Maximum = 16

🚀 Solution Approach:

Sort processorTime in ascending order.

Sort tasks in descending order.

For each processor:

Assign 4 tasks.

Compute processorTime[i] + tasks[i * 4]

Track the maximum.

Return the maximum.
