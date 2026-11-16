## 01. Convert String to Lower Case

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/convert-string-to-lowercase/1)

### Problem Description

**Task:** Given a string s, convert all its characters to lowercase.Examples:Input: s = "ABCddE"

#### Examples

##### Example 1

- **Output:**
```text
"lmnoppqq"
```
- **Explanation:** L, M, N, O, and Q are converted to l, m, n, o and q thus all uppercase characters of the string converted to lowercase letter.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-16 13:52:48
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string toLower(string& s) {
        // code here
         string ans="";
        for(int i=0;i<s.size();i++){
            ans.push_back(tolower(s[i]));
        }
        return ans;
    }
};
```

*Generated on: 11/16/2026, 1:53:13 PM*