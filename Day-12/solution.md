
# Day 12 Solution

## Approach

We use a **hash map (dictionary)** to count the frequency of each number.

Steps:

1. Create an empty dictionary.
2. Traverse through the array.
3. Increase the count of each number.
4. If any number count becomes greater than `n/2`, return that number.

---

## Code

```python
class Solution(object):
    def majorityElement(self, nums):

        freq = {}
        n = len(nums)

        for num in nums:
            freq[num] = freq.get(num, 0) + 1

            if freq[num] > n // 2:
                return num
