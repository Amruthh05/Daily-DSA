# Day 06 Solution

## Idea

We need to find the box with the **minimum capacity** that can still store the item.

Steps:

1. Go through each box in the capacity list.
2. Check if the box capacity is greater than or equal to the item size.
3. If yes, compare it with the current best answer.
4. Keep track of the index with the smallest valid capacity.
5. If no box can store the item, return -1.

---

## Code

```python
class Solution(object):
    def minimumIndex(self, capacity, itemSize):

        answer = -1

        for i in range(len(capacity)):
            if capacity[i] >= itemSize:
                if answer == -1 or capacity[i] < capacity[answer]:
                    answer = i

        return answer
