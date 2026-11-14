## 01. Reverse a String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-a-string/1)

### Problem Description

**Task:** Given a string s, reverse the string.Examples:Input: s = "Geeks"

#### Examples

##### Example 1

- **Output:**
```text
"skeeG"
```

##### Example 2

- **Input:**
```text
s = "for"
```
- **Output:**
```text
"a"
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 14:43:44
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string reverseString(string& s) {
        // code here
        int n=s.size();
        int i=0;
        int j=n-1;
        while(i<j){
            swap(s[i],s[j]);
            i++;
            j--;
        }
        
        
      return s;  
    }
};
```

*Generated on: 11/14/2026, 2:44:11 PM*