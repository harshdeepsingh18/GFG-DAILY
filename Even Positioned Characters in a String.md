## 01. Even Positioned Characters in a String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/for-loop-2/1)

### Problem Description

**Task:** Given a string s, return a string containing all characters present at even indices (0, 2, 4, ...). The characters must appear in the same order as in the original string.Examples: Input: s = "Geeks"

#### Examples

##### Example 1

- **Output:**
```text
DcoPeoea
```
- **Explanation:** The characters at even indices are collected in their original order.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-16 13:32:15
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string getEvenCharacters(string &s) {
        // code here
        string ans="";
        for(int i=0;i<s.length();i+=2){
            ans=ans+s[i];
        }
        return ans;
    }
};
```

*Generated on: 11/16/2026, 1:32:41 PM*