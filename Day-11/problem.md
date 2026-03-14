# Day 11

## Problem: Find Closest Person

Platform: LeetCode  
Problem Number: 3516  
Difficulty: Easy  
Topic: Math, Simulation

### Problem

We are given three integers `x`, `y`, and `z`.

- `x` is the position of **Person 1**
- `y` is the position of **Person 2**
- `z` is the position of **Person 3**

Person 3 does not move.

Both Person 1 and Person 2 move toward Person 3 at the **same speed**.

Our task is to determine **who reaches Person 3 first**.

Return:

- **1** → if Person 1 reaches first  
- **2** → if Person 2 reaches first  
- **0** → if both reach at the same time

---

### Example 1

Input  
x = 2  
y = 7  
z = 4  

Output  
1

Explanation  
Person 1 distance = |2 − 4| = 2  
Person 2 distance = |7 − 4| = 3  

Person 1 reaches first.

---

### Example 2

Input  
x = 2  
y = 5  
z = 6  

Output  
2

Explanation  
Person 1 distance = 4  
Person 2 distance = 1  

Person 2 reaches first.

---

### Example 3

Input  
x = 1  
y = 5  
z = 3  

Output  
0

Explanation  
Both distances are equal.
