
# Day 02

## Problem: Minimum Changes To Make Alternating Binary String

Platform: LeetCode  
Problem Number: 1758  
Difficulty: Easy  
Topic: String

### Problem

We are given a binary string `s` that contains only `0` and `1`.

In one operation, we can change any character:
- `0` to `1`
- or `1` to `0`

A string is called **alternating** if no two adjacent characters are the same.

Examples of alternating strings:
0101  
1010

Our task is to return the **minimum number of changes needed** to make the string alternating.

### Example 1

Input:  
s = "0100"

Output:  
1

Explanation:  
Changing the last character gives "0101", which is alternating.

### Example 2

Input:  
s = "10"

Output:  
0

Explanation:  
The string is already alternating.

### Example 3

Input:  
s = "1111"

Output:  
2

Explanation:  
We can convert it to "1010" or "0101".
