
# Day 03 Solution

## Idea

First convert the number into its **binary string**.

Python provides `bin()` function to convert a number to binary.

Example:
bin(5) → '0b101'

We remove `0b` using `[2:]`.

Then we check each pair of adjacent bits.

If two neighbouring bits are the same, then the number does not have alternating bits.

If we reach the end without finding equal adjacent bits, then it is alternating.

## Code

```python
class Solution(object):
    def hasAlternatingBits(self, n):

        n = bin(n)[2:]
        arr = n

        for i in range(len(arr)-1):
            if arr[i] == arr[i+1]:
                return False

        return True
