
# Day 02 Solution

## Idea

An alternating binary string can have only two possible patterns:

Pattern 1:  
010101...

Pattern 2:  
101010...

We count how many changes are needed to convert the given string into each pattern.

- `pattern1` counts changes needed for "010101..."
- `pattern2` counts changes needed for "101010..."

For each index:
- If index is even → expected character is different for each pattern
- If index is odd → expected character is opposite

At the end we return the **minimum changes** between the two patterns.

## Code

```python
class Solution(object):
    def minOperations(self, s):

        pattern1 = 0   # for 010101...
        pattern2 = 0   # for 101010...

        for i in range(len(s)):

            if i % 2 == 0:
                if s[i] != '0':
                    pattern1 += 1
                if s[i] != '1':
                    pattern2 += 1
            else:
                if s[i] != '1':
                    pattern1 += 1
                if s[i] != '0':
                    pattern2 += 1

        return min(pattern1, pattern2)
