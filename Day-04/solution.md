# Day 04 Solution

## Idea

We need to check how many **segments of '1's** appear in the string.

A new segment of ones starts when:
- the current character is '1'
- and the previous character is '0'
- or the index is 0

So we count how many times a new segment of ones starts.

If the count is **greater than 1**, then the string has multiple segments of ones and the answer is false.

Otherwise, it is true.

## Code

```python
class Solution(object):
    def checkOnesSegment(self, s):

        count = 0

        for i in range(len(s)):
            if s[i] == '1':
                if i == 0 or s[i-1] == '0':
                    count += 1

        ans = count <= 1
        return ans
