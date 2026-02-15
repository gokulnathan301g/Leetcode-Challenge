Problem: Remove Duplicates from Sorted List (LeetCode #83)

Difficulty: Easy
Language: Java
Topic: Linked List

Problem Statement:
Given the head of a sorted linked list, delete all duplicates such that each element appears only once.

Return the linked list sorted as well.

Example:

Input: head = [1,1,2]
Output: [1,2]
Explanation:
Duplicate 1 is removed.


Input: head = [1,1,2,3,3]
Output: [1,2,3]
Explanation:
Duplicates 1 and 3 are removed.


Solution:

Initialize a pointer curr to the head of the linked list.

Traverse the list while curr and curr.next are not null.

If the current node value equals the next node value, skip the duplicate by updating curr.next.

Otherwise, move curr to the next node.

Continue until the end of the list.

Return the modified head of the linked list.
