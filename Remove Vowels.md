## 01. Remove Vowels

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-vowels-from-string1446/1)

### Problem Description

**Task:** Given a string s. Your task is to remove the vowels from the string.

#### Examples

##### Example 1

- **Input:**
```text
s = "welcome to geeksforgeeks"
```
- **Output:**
```text
"wlcm t gksfrgks"
```
- **Explanation:** Vowels were ignored only consonents were returned in the same order.

##### Example 2

- **Input:**
```text
s = "what is your name ?"
```
- **Output:**
```text
wht s yr nm ?
```

#### Constraints

- **1.** `1 <= |s| <= 10⁵Alphabets are lower cases only`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-11-16 15:27:10
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    string removeVowels(string& s) {
        // code here
        string ans="";
        for(int i=0;i<s.size();i++){
            if(s[i]!='a' &&
             s[i]!='i' &&
             s[i]!='e' &&
             s[i]!='u' &&
             s[i]!='o' ){
                  
                  ans.push_back(s[i]);
             }
            
            
        }
        return ans;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-11-16 15:26:56
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string removeVowels(string& s) {
        // code here
        string ans="";
        for(int i=0;i<s.size();i++){
            if(s[i]!='a' &&
             s[i]!='i' &&
             s[i]!='e' &&
             s[i]!='u' &&
             s[i]!='o' ){
                  
                  ans.push_back(s[i]);
             }
            
            
        }
        return ans;
    }
};
```

*Generated on: 11/16/2026, 3:27:24 PM*