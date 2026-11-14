## 01. Longest Word

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/display-longest-name0853/1)

### Problem Description

**Task:** Given an array arr[] containing strings of names. Your task is to return the longest string. If there are multiple names of the longest size, return the first occurring name.Examples :Input: arr[] = ["Geek", "Geeks", "Geeksfor", "GeeksforGeek", "GeeksforGeeks"]

#### Examples

##### Example 1

- **Output:**
```text
"GeeksforGeeks"Explanation: Name "GeeksforGeeks" has maximum length among all names. Input: arr[] = ["Apple", "Mango", "Orange", "Banana"]Output: "Orange"Explanation: Names "Orange" and "Banana" both have maximum length among all names but Orange comes first so answer will be "Orange".
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-14 22:54:43
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    string longest(vector<string>& arr) {
        // code here
         string ans="";
        for(int i=0;i<arr.size();i++){
            if(arr[i].size()>ans.size()){
                ans=arr[i];
            }
        }
        return ans;
    }
};
```

*Generated on: 11/14/2026, 10:57:06 PM*