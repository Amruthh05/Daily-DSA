# Day 09 Solution

## Idea

The idea is simple.

1. Convert the digit array into a number.
2. Add 1 to the number.
3. Convert the number back into digits.
4. Return the result as a list.

---

## Code

```python
class Solution(object):
    def plusOne(self, digits):

        num = 0

        for d in digits:
            num = num * 10 + d

        num += 1

        result = []

        for ch in str(num):
            result.append(int(ch))

        return result
