# Day 08 Solution

## Idea

The idea is simple.

1. Traverse the array.
2. Store all non-zero elements in a temporary list.
3. Count how many zeros appear.
4. Append the zeros at the end of the temporary list.
5. Copy the result back to the original array.

This maintains the order of the non-zero elements.

---

## Code

```python
class Solution(object):
    def moveZeroes(self, nums):

        temp = []
        zeros = 0

        for i in nums:
            if i == 0:
                zeros += 1
            else:
                temp.append(i)

        for zero in range(zeros):
            temp.append(0)

        for j in range(len(nums)):
            nums[j] = temp[j]
