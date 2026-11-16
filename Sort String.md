## 01. Sort String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sort-a-string2943/1)

### Problem Description

**Task:** Given a string consisting of lowercase letters, arrange all its letters in ascending order. Examples:Input: s = "edcab"

#### Examples

##### Example 1

- **Output:**
```text
"abcde"
```
- **Explanation:** characters are in ascending order in "abcde".

##### Example 2

- **Input:**
```text
s = "xzy"
```
- **Output:**
```text
"xyz"
```
- **Explanation:** characters are in ascending order in "xyz".

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(|s|)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-16 16:42:00
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string sortString(string &s) {
        // code here
        sort(s.begin(),s.end());
        return s;
        
    }
};
```

*Generated on: 11/16/2026, 4:42:28 PM*