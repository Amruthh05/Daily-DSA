
# Day 07

## Problem: Partition Array According to Given Pivot

Platform: LeetCode  
Problem Number: 2161  
Difficulty: Medium  
Topic: Arrays

### Problem

We are given an integer array `nums` and an integer `pivot`.

We need to rearrange the array based on the pivot value.

The final array should follow these rules:

1. All elements **less than pivot** should appear first.
2. All elements **equal to pivot** should appear next.
3. All elements **greater than pivot** should appear last.

Important:  
The **relative order of elements must stay the same** inside each group.

---

### Example 1

Input  
nums = [9,12,5,10,14,3,10]  
pivot = 10  

Output  
[9,5,3,10,10,12,14]

Explanation  
Numbers less than pivot → [9,5,3]  
Numbers equal to pivot → [10,10]  
Numbers greater than pivot → [12,14]

---

### Example 2

Input  
nums = [-3,4,3,2]  
pivot = 2  

Output  
[-3,2,4,3]
