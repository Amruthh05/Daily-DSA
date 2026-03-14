
# Day 11 Solution

## Idea

We simply compare the **distance of Person 1 and Person 2 from Person 3**.

Distance formula:

distance = |position − target|

Steps:

1. Calculate distance from Person 1 to Person 3.
2. Calculate distance from Person 2 to Person 3.
3. Compare the distances.

- If distance1 < distance2 → return 1
- If distance2 < distance1 → return 2
- Otherwise → return 0

---

## Code

```python
class Solution(object):
    def findClosest(self, x, y, z):

        distance1 = abs(x - z)
        distance2 = abs(y - z)

        if distance1 < distance2:
            return 1
        elif distance2 < distance1:
            return 2
        else:
            return 0
