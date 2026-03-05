# Day 03

## Problem: Binary Number with Alternating Bits

Platform: LeetCode  
Problem Number: 693  
Difficulty: Easy  
Topic: Bit Manipulation

### Problem

We are given a positive integer `n`.

We need to check whether the **binary representation** of this number has **alternating bits**.

Alternating bits means:
No two adjacent bits are the same.

Example of alternating bits:
101  
1010  
0101

If two neighbouring bits are equal like **11 or 00**, then it is not alternating.

Return **true** if the number has alternating bits, otherwise return **false**.

### Example 1

Input:  
n = 5  

Output:  
true  

Explanation:  
Binary representation of 5 is **101**, which is alternating.

### Example 2

Input:  
n = 7  

Output:  
false  

Explanation:  
Binary representation of 7 is **111**, which is not alternating.

### Example 3

Input:  
n = 11  

Output:  
false  

Explanation:  
Binary representation of 11 is **1011**.  
The last two bits are the same, so it is not alternating.
