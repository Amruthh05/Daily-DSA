
# Day 10 Solution

## Idea

We use a **set** to track numbers that we have already seen.

Steps:

1. Create an empty set.
2. Traverse the list.
3. If a number already exists in the set, it means it appeared before → add it to the answer.
4. Otherwise add it to the set.

---

## Code

```python
class Solution(object):
    def getSneakyNumbers(self, nums):

        seen = set()
        answer = []

        for i in nums:
            if i in seen:
                answer.append(i)
            else:
                seen.add(i)

        return answer
