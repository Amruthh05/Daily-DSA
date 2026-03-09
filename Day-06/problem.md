# Day 06

## Problem: Minimum Capacity Box

Platform: LeetCode  
Problem Number: 3861  
Difficulty: Easy  
Topic: Arrays

### Problem

We are given an array `capacity` where `capacity[i]` represents the capacity of the ith box.

We are also given an integer `itemSize` which represents the size of an item.

A box can store the item if:

capacity[i] >= itemSize

Our task is to return the **index of the box with the minimum capacity that can store the item**.

If multiple boxes satisfy the condition, return the **smallest index**.

If no box can store the item, return **-1**.

---

### Example 1

Input  
capacity = [1,5,3,7]  
itemSize = 3

Output  
2

Explanation  
Box at index 2 has capacity 3 which is the minimum capacity that can store the item.

---

### Example 2

Input  
capacity = [3,5,4,3]  
itemSize = 2

Output  
0

Explanation  
Minimum capacity that can store the item is 3.  
It appears at index 0 and index 3, so we return index 0.
