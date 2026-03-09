
# Day 07 Solution

## Idea

We divide the array into three groups:

1. Numbers smaller than the pivot
2. Numbers equal to the pivot
3. Numbers greater than the pivot

We store them in three separate lists.

Then we combine the lists in the order:
smaller + equal + greater.

This keeps the relative order of elements.

---

## Code

```python
class Solution(object):
    def pivotArray(self, nums, pivot):

        arrMin = []
        arrEqual = []
        arrMax = []

        for i in nums:
            if i < pivot:
                arrMin.append(i)
            elif i == pivot:
                arrEqual.append(i)
            else:
                arrMax.append(i)

        result = arrMin + arrEqual + arrMax
        return result
