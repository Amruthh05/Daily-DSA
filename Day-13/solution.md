
# Day 13 Solution

## Approach

We use a **list (or set)** to keep track of seen characters.

Steps:

1. Traverse through the string.
2. If the character is already seen → return it.
3. Otherwise add it to the seen list.

---

## Code

```python
class Solution(object):
    def repeatedCharacter(self, s):

        seen = []

        for char in s:
            if char in seen:
                return char
            else:
                seen.append(char)
