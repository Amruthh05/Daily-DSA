# Day 09 - Problem 2 Solution

## Idea

We use a **set** to track numbers we have already seen.

Steps:

1. Create an empty set.
2. Traverse the array.
3. If the number already exists in the set → return True.
4. Otherwise add the number to the set.
5. If the loop finishes, return False.

---

## Code

```python
class Solution(object):
    def containsDuplicate(self, nums):

        result = set()

        for i in nums:
            if i in result:
                return True
            result.add(i)

        return False
