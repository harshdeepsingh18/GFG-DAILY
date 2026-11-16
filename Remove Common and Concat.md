## 01. Remove Common and Concat

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/remove-common-characters-and-concatenate-1587115621/1)

### Problem Description

**Task:** Given two strings, s1 and s2. The task is to remove all characters that are common in both strings and then combine the remaining characters from each string to form a new string.
The characters that are not shared between the two strings should appear in the result in the same order as they appear in their respective original strings.
If no characters are left after removing the common characters, return "-1"

#### Examples

##### Example 1

- **Input:**
```text
s1 = aacdb, s2 = gafd
```
- **Output:**
```text
cbgf
```
- **Explanation:** The common characters of s1 and s2 are: a, d. The uncommon characters of s1 and s2 are c, b, g and f. Thus the modified string with uncommon characters concatenated is cbgf.

##### Example 2

- **Input:**
```text
s1 = abcs, s2 = cxzca
```
- **Output:**
```text
bsxz
```
- **Explanation:** The common characters of s1 and s2 are: a,c. The uncommon characters of s1 and s2 are b,s,x and z. Thus the modified string with uncommon characters concatenated is bsxz.

#### Constraints

- **1.** `1 <= |Length of Strings| <= 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-16 15:14:08
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string concatenatedString(string &s1, string &s2) {
        //  code here
        int freq1[26]={0};
        int freq2[26]={0};
        for(int i=0;i<s1.size();i++){
            freq1[s1[i]-'a']=1;
        }
        for(int i=0;i<s2.size();i++){
            freq2[s2[i]-'a']=1;
        }
        string ans="";
        
        for(int i=0;i<s1.size();i++){
             if(freq2[s1[i] -'a']==0){
                 ans=ans+s1[i];
             }
             
        }         
                     
          for(int i=0;i<s2.size();i++){
                   if(freq1[s2[i] -'a']==0){
                 ans=ans+s2[i];
             }
             
             
            }
            if(ans==""){
                return "-1";
            }
            
            return ans;
    }
};
```

*Generated on: 11/16/2026, 3:14:33 PM*