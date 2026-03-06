# Day 04

## Problem: Check if Binary String Has at Most One Segment of Ones

Platform: LeetCode  
Difficulty: Easy  
Topic: String

### Problem

We are given a binary string `s` that contains only `0` and `1`.

The string has **at most one segment of ones** if all the `1`s appear together in a single continuous block.

If there are multiple separated groups of `1`s, then the condition is not satisfied.

Return **true** if the string contains **at most one contiguous segment of ones**, otherwise return **false**.

### Example 1

Input:  
s = "1001"

Output:  
false

Explanation:  
The ones are separated, so they are not a single segment.

### Example 2

Input:  
s = "110"

Output:  
true

Explanation:  
All the ones are together in one segment.

### Constraints

- 1 <= s.length <= 100
- s contains only '0' and '1'
- s does not contain leading zeros
