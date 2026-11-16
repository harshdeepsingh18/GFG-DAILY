## 01. Check Palindrome Ignoring Case

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-palindrome--141628/1)

### Problem Description

**Task:** Given a string s consisting only of English alphabets, check whether it is a palindrome or not, ignoring the case of the letters. A string is a palindrome if it reads the same forward and backward when case differences are ignored. Return true if s is a palindrome, otherwise return false.Examples:Input: s = "Hello"

#### Examples

##### Example 1

- **Output:**
```text
true
```
- **Explanation:** TenEt = = tEneT as we are ignoring the case.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-16 15:41:28
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    bool isPalindrome(string& s) {
        // code here
        int flag=true;
        int i=0;
        int j=s.size()-1;
        
        while(i<j){
            
            if(tolower(s[i])!=tolower(s[j])){
              flag=false;  
              break;
            }
            i++;
            j--;
        }
        return flag;
    }
};
```

*Generated on: 11/16/2026, 3:42:06 PM*