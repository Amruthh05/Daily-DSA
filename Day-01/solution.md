
# Day 01 Solution

## Idea

At first we could try checking every pair of numbers using two loops, but that would take O(n²) time.

A better way is to use a **dictionary (hash map)**.

The idea is to store numbers we have already seen along with their index.

For every number in the array:
1. Find the value needed to reach the target.
2. Check if that value is already in the dictionary.
3. If it is, we found the answer.
4. If not, store the current number and its index.

This way we only go through the array once.

## Code

```python
class Solution(object):
    def twoSum(self, nums, target):

        result = {}

        for i, num in enumerate(nums):
            difference = target - num

            if difference in result:
                return [i, result[difference]]

            result[num] = i

        return None
