
# Day 05 Solution

## Idea

The idea is simple.

1. Convert the binary strings into decimal numbers.
2. Add the two numbers.
3. Convert the result back to binary.

Python provides built-in functions for this.

- `int(x, 2)` converts binary to decimal
- `bin(x)` converts decimal to binary

`bin()` returns a string starting with **0b**, so we remove it using `[2:]`.

---

## Code

```python
class Solution(object):
    def addBinary(self, a, b):

        new_a = int(a, 2)
        new_b = int(b, 2)

        total = new_a + new_b

        result = bin(total)[2:]

        return result
